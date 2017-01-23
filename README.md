# NodejsSpeechTranslateApp

The sample code is designed to illustrate the 2 methods supported in the Microsoft Translater API
1. calling /languages to get the list of supported languages for speech, text and text to speech
2. calling /speech/translate to get the recognition and translation of an audio file.  the audio file is in PCM 16bit, 16kHz mono WAV format (with header)

## Instructions
1. To get the package dependencies, first execute "npm install"
2. Edit app.js and enter your Azure Key API
var azureApiKey = '[azure Api Key]';
3. Run by executing "node app.js"

If you want to change the audio file, simply change the line 
var file = 'helloworld.wav';

## Dependencies
request, stream-buffers, websocket

####Getting Started
-You will need to setup a subscription with Microsoft Translator. [Click Here] (https://portal.azure.com) to get started.

-More Infos about Tokens: [Click Here] (http://docs.microsofttranslator.com/oauth-token.html)

-Speech API documentation can be [found here.] (http://docs.microsofttranslator.com/speech-translate.html)
This app posts translations to a webservice. You will need a website to post to, or change the app to post locally to the UIWebView.
