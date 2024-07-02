# application
//python based speech to text converting application
import speech recognisation as sr
AUDIO_FILE=("sample_simran.nav")
r=sr.recogniser()
with sr.audiofile (AUDIO_FILE)as sources:
audio=r.record(source)
try:
pringt("audio file contain"+r.recognise_google(audio))
except sr.unknownValueError:
print("google speech recognisation could nt understand audio")
except sr.RequestError:
print("could not get result from google speech recognistaion")
