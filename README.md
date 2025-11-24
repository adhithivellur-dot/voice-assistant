# Scuba voice Assistant 🎤
A Python-based voice assistant that can respond to voice commands, answer questions, tell jokes, and perform various tasks through speech recognition and text-to-speech capabilities.
## Features
Voice Recognition: Listens and processes voice commands using Google Speech Recognition

Text-to-Speech: Responds with a natural-sounding voice

Time Information: Tells the current time when asked

Web Navigation: Opens YouTube on command

Entertainment: Tells science-themed jokes

Personal Information: Responds to questions about its name and age

Wake Word Activation: Activates when you say "Hey Scuba"

## Prerequisites
Before running the project, ensure you have Python 3.7+ installed on your system.
### Installation

Clone the repository:

bashgit clone https://github.com/yourusername/scuba-voice-assistant.git
cd scuba-voice-assistant

Install the required dependencies:

bashpip install pyttsx3

pip install SpeechRecognition

pip install pyjokes

pip install pyaudio

Note for PyAudio installation issues:

Windows: Download the appropriate .whl file from here and install using pip install filename.whl

Linux: Run sudo apt-get install python3-pyaudio

Mac: Run brew install portaudio then pip install pyaudio

### Usage

Run the voice assistant:

bashpython voice_assistant.py

Say "Hey Scuba" to activate the assistant

Use the following voice commands:

"What's your name?" - Get the assistant's name

"How old are you?" - Get the assistant's age

"What time is it?" - Get the current time

"Open YouTube" - Opens YouTube in your browser

"Tell me a joke" - Hear a science joke

"Exit" - Close the assistant


## Dependencies

pyttsx3: Text-to-speech conversion library

SpeechRecognition: Library for performing speech recognition

webbrowser: Opens web pages (built-in)

datetime: Handles date and time operations (built-in)

pyjokes: Generates programming jokes

pyaudio: Audio I/O library for recording audio

## How It Works

The program initializes and waits for the wake word "Hey Scuba"
Once activated, it continuously listens for voice commands
Commands are processed using Google Speech Recognition API
Responses are generated and spoken back using pyttsx3
The assistant continues listening until you say "exit"

## Limitations

1.Requires an active internet connection for speech recognition

2.Microphone access is required

3.Background noise may affect recognition accuracy

4.Google Speech Recognition API has usage limits

## Future Enhancements
 1. Add weather information feature
   
 2.Integration with calendar and reminders
   
 3.Smart home device control
 
 4. Music playback control
   
 5.Email and message reading
 
 6.News headlines retrieval
 

## Troubleshooting
Microphone not detected:

Ensure your microphone is properly connected
Check system permissions for microphone access
Try running the script with administrator/sudo privileges

Speech recognition errors:

Speak clearly and at a moderate pace
Reduce background noise
Check your internet connection
Adjust the adjust_for_ambient_noise() timeout if needed

Voice sounds robotic:

Adjust the speech rate in the code (currently set to 150)
Try different voice options available in pyttsx3

