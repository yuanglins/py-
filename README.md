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

#青蛙寻妈
import playsound
from aip import AipSpeech

""" 你的 APPID AK SK """
APP_ID = '24237604'
API_KEY = 'BSsWyIgnzBdW3GQomzAWomTB'
SECRET_KEY = 'tGrgDb2IoPFCyDGmYqoGPS02BOGfTBUE'
client = AipSpeech (APP_ID, API_KEY, SECRET_KEY)

animals = ['鸭', '鱼', '乌龟', '鹅', '青蛙', '虾', '鳄鱼']
for each in animals:
    print("请问你是我妈妈吗？")
    result  = client.synthesis("请问你是我妈妈吗？", 'zh', 1, {'vol': 5,})
    if not isinstance(result, dict):
        with open('audio.mp3', 'wb') as f:
            f.write(result)
        playsound.playsound('audio.mp3')

    if each != "青蛙":
        print ('我是'+ each +',我不是你妈妈。','zh',1,{'vol': 5,})
        result  = client.synthesis('我是'+each + "，我不是你妈妈。", 'zh', 1, {'vol': 5,})
        if not isinstance(result, dict):
            with open('audio1.mp3', 'wb') as f:
                f.write(result)
        playsound.playsound('audio1.mp3')

    else:
        print ('我是青蛙：我是你妈妈.')
        result  = client.synthesis('我是'+each + "，我不是你妈妈。", 'zh', 1, {'vol': 5,})
        if not isinstance(result, dict):
            with open('audio2.mp3', 'wb') as f:
                f.write(result)
        playsound.playsound('audio2.mp3')

        break
