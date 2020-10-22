# Micro-bit-Project
This is my micro:bit project meant to encourage students during exam period. Please feel free to improve this code with pull requests! 

from microbit import * 
#This is my second (final) code 
while True:
  if button_b.is_pressed() and button_a.is_pressed():
    display.show(Image.SILLY)
    display.clear()
  elif button_a.was_pressed():
    display.scroll("We all")
    display.show(Image.HEART)
    sleep(1000)
    display.scroll("you!")
  elif button_b.was_pressed():
    display.scroll("Remember to")
    display.show(Image.HEART)
    sleep(1000)
    display.scroll("yourself too!")
  else:
    display.show(Image.HEART, wait = False)
    sleep(500)
    display.clear()
    display.show(Image.HEART_SMALL, wait = False)
    sleep(500)
    display.clear()
