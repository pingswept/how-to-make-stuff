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

Setting up student accounts didn't work so well. Not sure what went wrong. Here was the reply from Amazon:

    I am following up with your Educate enquiry regarding your students' accounts.
    In order for students to activate their starter account, they have to activate their starter accounts via the link sent to them in their welcome email. Students must not create an AWS account.
    The link in their welcome email provides directions on how to set up their starter account.
    Please let me know if your students received their welcome email.
    I can resend them their welcome emails to ensure they are correctly set up.

Instead, just ran 10 instances on my account, gave students access to them. Had to set password and enable password authentication for `sshd`.

Username: ubuntu

    sudo nano /etc/ssh/sshd_config

    PasswordAuthentication yes

    sudo service sshd restart
    sudo passwd ubuntu
