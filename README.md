#this micropython file uses only internal commands so there is no dependentsies on imports and it is long habd easy to understand and edit.. it represents 
#100 hours of research to trry to figure outr rthe internal commands and structurs so that it is very easy to understand edit and usa as a temnplate. thanks 
#for reading. below is an earlier version of the script. the latest one uses an if astatement and has a different execuition order
# jsj_pico_pi_25_blinkking_led
# pico pi micropython all internal commands 25 blinking led one input 
# button
# 0https://wokwi.com/projects/368213601376419841
p=0
i=0
c=0
d=5
a=1
l=1
jsjs=0
k=0
b=0
#
print(" initalize gpio pins")
#
for i in range(29):
    print(i," ",end="" )   
    machine.Pin(i, machine.Pin.OUT)
#
print("number of loops")
while l:
    for p in range(26):
        p=p+3*(p>22)
        machine.Pin(p).value(a)
        machine.lightsleep(d)
        machine.Pin(p).value(0)
        d=int(d*(d<1000)+(d/5)*(b==0)*(k==1)+5*(d<5))
        b=k
        machine.Pin(28, machine.Pin.IN)
        k=machine.Pin(28).value()
        machine.Pin(28, machine.Pin.OUT)
    print(" ",jsjs," ",d,end="")
    jsjs=jsjs+1
