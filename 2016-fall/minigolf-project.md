Python code to run on Amazon EC2

    from flask import Flask
    app = Flask('test-application')

    score=0 # create global variable for persistent storage

    @app.route('/test')
    def hello_world():
        return 'Hello World!!'

    @app.route('/score')
    def report_score():
        global score
        return str(score)

    @app.route('/score/add/<number>')
    def add_to_score(number):
        global score
        score = score + int(number) # variables pulled from URLs are strings, so int() makes it an integer
        return 'Current score is: {0}'.format(score)

    if __name__ == "__main__":
        app.run(host='0.0.0.0', port=80, debug=True)

C++ code to run on Particle Photon. Increments score by 100 points every 10 seconds.

    #include "HttpClient/HttpClient.h"

    unsigned int nextTime = 0;    // Next time to contact the server
    HttpClient http;

    http_header_t headers[] = {
        { "Accept" , "*/*"},
        { NULL, NULL } // NOTE: Always terminate headers with NULL
    };

    http_request_t request;
    http_response_t response;

    void setup() {
        Serial.begin(9600);
        request.hostname = "54.159.177.56";
        request.port = 80;
        request.path = "/score/add/100";
    }

    void loop() {
        if (nextTime > millis()) {
            return;
        }

        http.get(request, response, headers);

        Serial.print("Response status: ");
        Serial.println(response.status);

        Serial.print("HTTP response body: ");
        Serial.println(response.body);

        nextTime = millis() + 10000; // set nextTime to be 10 seconds in the future
    }

On a Mac, if your Photon is connected to the USB port, you can listen to the Photon's serial messages using `screen`.

    screen /dev/tty.usbmodemFA141 9600

On Windows, you could create a similar 9600 bps serial connection using Putty.
