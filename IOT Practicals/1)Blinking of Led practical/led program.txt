import RPi.GPIO as GPIO
import time

GPIO.setmode(GPIO.BOARD)
GPIO.setup(7,GPIO.OUT)
GPIO.setup(11,GPIO.OUT)
GPIO.setup(13,GPIO.OUT)
GPIO.setup(15,GPIO.OUT)

for i in range(10):
    GPIO.output(7,True)
    print("LED on")
    time.sleep(4)
    GPIO.output(7,False)
    print("LED off")
   
    
    GPIO.output(11,True)
    print("LED on")
    time.sleep(3)
    GPIO.output(11,False)
    print("LED off")
    
    
    GPIO.output(13,True)
    print("LED on")
    time.sleep(2)
    GPIO.output(13,False)
    print("LED off")
   
    
    GPIO.output(15,True)
    print("LED on")
    time.sleep(1)
    GPIO.output(15,False)
    print("LED off")
    
    
print("Done..")
GPIO.cleanup()