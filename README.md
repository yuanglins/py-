# py-
py作品
#1 .用百度AI读新闻
import os
from aip import AipSpeech

""" 你的 APPID AK SK """
APP_ID = '24237604'
API_KEY = 'BSsWyIgnzBdW3GQomzAWomTB'
SECRET_KEY = 'tGrgDb2IoPFCyDGmYqoGPS02BOGfTBUE'

client = AipSpeech (APP_ID, API_KEY, SECRET_KEY)

NEWS=input('新闻：')
result  = client.synthesis(NEWS, 'zh', 1, {'vol': 5,})
if not isinstance(result, dict):
    with open('audio.mp3', 'wb') as f:
        f.write(result)
    os.system('audio.mp3')
