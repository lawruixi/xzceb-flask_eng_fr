# Flask Translator App

## Introduction
Greetings! It is I, back again with another mind-blowing project. Let's get right into it.

This App is a web app with Flask backend, that aims to help you translate text from English to French and vice-versa. This text must be sufficiently long (i.e. nonzero length). This Translator app uses the IBM Watson Language Translator service. The webpage will be updated with the translated text once it receives the response.

## Installation
Firstly, we need the following:

- `pip`
- `python3`
- `flask`
- `ibm-watson`
- `python-dotenv`

Install them as follows (using your distribution's package managers as necessary):
```bash
$> sudo apt update && sudo apt install python3 python3-pip
```
```bash
$> pip3 install flask ibm-watson python-dotenv
```

Now git clone the project:
```bash
$> git clone https://github.com/lawruixi/xzceb-flask_eng_fr
$> cd xzceb-flask_eng_fr
```

At this stage, we'll be needing the Language Translator service from IBM, so head on over [there](https://cloud.ibm.com/catalog/services/language-translator) to get it. Once again, no, I'm not sharing my API credentials. It's free anyway, and you can always unsubscribe later. 

Once you have set up the service, go to Resource List > Language Translator > Manage to view your API credentials.
```
$> touch .env
$> echo "apikey=<API key>" >> .env
$> echo "url=<URL>" >> .env
```

And that's all.

## Usage
Start the flask app:
```
python3 server.py
```
And visit the webpage (probably `localhost:8080`) using your browser (or `cURL` if you're that kinda person). Alternatively, you can visit [this website](http://lawruixi3v3translationapp.mybluemix.net/) (which I cannot guarantee will be up for long, due to the nature of IBM Cloud Trial Account and me using their IBM Service Lite Plan). Have fun playing around!

## Acknowledgements
Once upon a time, there was a young student who was programming. This student decided to, for the sake of having a professional-looking certificate on their resumé, enroll in online courses to boost their employment chances in the future. This student stumbled upon one such course, which promised to this student that they could achieve programming heights never before dreamed of. And thus began this student's journey into the unknown and learning about new technologies that are emerging today. At the end of this course, the student was faced with a project. And when they finished their final project, they leaned back with a satisfied sigh, as she proclaimed:

"Thank you to the Final Project in the [Python Project for AI and Application Development Course](https://www.coursera.org/learn/python-project-for-ai-application-development) as part of the [IBM Full Stack Cloud Developer Professional Certificate](https://www.coursera.org/professional-certificates/ibm-full-stack-cloud-developer) on [Coursera](https://www.coursera.org/), without which I couldn't possibly have come this far. Shoutout to you!"

<sup><sub>I like how that's the longest section in this README</sub></sup>
