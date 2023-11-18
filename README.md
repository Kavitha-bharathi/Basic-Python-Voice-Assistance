# Basic-Python-Voice-Assistance
#this code works using internet connection

import os
import time
import playsound
import speech_recognition as sr
from gtts import gTTS 

def speak(text):
    tts=gTTS(text=text,lang='en')
    filename='sound.mp3'
    tts.save(filename)
    playsound.playsound(filename)
speak('welcome to learn python')
print('done')

