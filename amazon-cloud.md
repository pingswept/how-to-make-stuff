Create student accounts at https://www.awseducate.com/Application

    ssh -i ~/path/to/private-key.pem ubuntu@54.163.191.47

    sudo apt-get install python-flask

Save as test.py:

    from flask import Flask
    app = Flask('test-application')

    @app.route('/test')
    def hello_world():
        return 'Hello World!'

List processes listening to the internet

    netstat -lnt

Run the Flask app.

    sudo python -i test.py
    >>> app.run(host='0.0.0.0', port=80)
