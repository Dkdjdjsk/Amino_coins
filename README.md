# Amino_coins
B = '\033[1;30m'
r = '\033[1;31m'
c = '\033[1;36m'
g = '\033[0;32m'
y = '\033[1;33m'
B = '\033[4;30m'
er = '\033[1;34m'

import time
import sys
import amino
from hashlib import sha1
import base64
import string
import random
def device():
 S=1000
 ran = ''.join(random.choices(string.ascii_uppercase + string.digits, k = S))  
 m='01' + (hardwareInfo := sha1(ran.encode("utf-8"))).hexdigest() + sha1(bytes.fromhex('01') + hardwareInfo.digest() + base64.b64decode("6a8tf0Meh6T4x7b0XvwEt+Xw6k8=")).hexdigest()
clint=amino.Client(deviceId=device())

print (g+"""

              _                  ______                           __            
  _________  (_)___  _____      / ____/__  ____  ___  _________ _/ /_____  _____
 / ___/ __ \/ / __ \/ ___/_____/ / __/ _ \/ __ \/ _ \/ ___/ __ `/ __/ __ \/ ___/
/ /__/ /_/ / / / / (__  )_____/ /_/ /  __/ / / /  __/ /  / /_/ / /_/ /_/ / /    
\___/\____/_/_/ /_/____/      \____/\___/_/ /_/\___/_/   \__,_/\__/\____/_/     

	                  			""",c+"fajer-alhacker")


print("\n")
print("\n")

paso=input("\033[1;31m# password : \033[1;0m")

print("Loading:")

a="              "
animation = ["[■□□□□□□□□□]","[■■□□□□□□□□]", "[■■■□□□□□□□]", "[■■■■□□□□□□]", "[■■■■■□□□□□]", "[■■■■■■□□□□]", "[■■■■■■■□□□]", "[■■■■■■■■□□]", "[■■■■■■■■■□]", "[■■■■■■■■■■]"]

for i in range(len(animation)):
    time.sleep(0.7)
    sys.stdout.write("\r" + animation[i % len(animation)])
    sys.stdout.flush()

print("\n")

from datetime import datetime
def magicnum():
    toime={"start":int(datetime.timestamp(datetime.now())),"end":int(datetime.timestamp(datetime.now()))+300}
    return toime
print(magicnum())
timer=[
magicnum(),magicnum(),magicnum(),magicnum(),magicnum(),magicnum(),magicnum(),magicnum(),magicnum(),magicnum(),magicnum(),magicnum()
,magicnum(),magicnum(),magicnum(),magicnum(),magicnum(),magicnum(),magicnum(),magicnum(),magicnum(),magicnum(),magicnum(),magicnum(),
magicnum(),magicnum(),magicnum(),magicnum(),magicnum(),magicnum(),magicnum(),magicnum(),magicnum(),magicnum(),magicnum(),magicnum()
]
start=0
for e in open("/sdcard/email.txt").read().split():
 clint.login(email=e,password=paso)
 spreso=clint.sub_clients(start=0,size=200).comId
 print(spreso)
 spreso=str(spreso)
 spreso=spreso.count(",")
 spreso+=1
 print(spreso)
 for kb in range(spreso):
  sub=amino.SubClient(comId=clint.sub_clients( start=start , size=spreso ).comId[0],profile=clint.profile)
  sub.activity_status("on")
  sub.send_active_obj(timers=timer)
  start+=1
  print(g+"logged in ","\033[1;31m|"  ,"\033[1;0m" +e ,  "\033[1;31m|")
