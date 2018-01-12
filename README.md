import random
import time

def displayIntro () :
    print ("It is the end of a hard year fighting criminals")
    print ("you visit different places and crossroads before you get back in your place")
    print ("where you will see your favourite things")
    print ("if you pick the wrong path you will suffer")
    print ()

def choosePlace () :
    path = ""
    while place != "1" and path !="2" # input validation
    path = input("Which place would you prefer?  (1 or 2) : ")

    return place

def checkPlace(choosenplace) :
    print ("you walk through a crowded alley")
    time.sleep(3)
    print ("you see a beautiful lady")
    time.sleep(4)
    print ("but then your skin starts to itch")
    print ()
    time.sleep(2)

    correctPlace = random.randit(1, 2)

    if choosenPlace == correctPlace:
        print ("the itching was the urge for talking to the woman and going back home for a cup of tea")
        print ("Welcome back to your room")
    else:
        print ("you have been stabbed by the woman multiple time and left on the street")
        print ("and everybody is laughing at you while you are suffering before kicking the bucket")


playAgain = "yes"
  while playAgain == "yes" or playAgain = "y":
      displayIntro()
      choice = choosenPlace()
      checkPlace(choice) # coice is equal to "1" or "2"
      playAgain input("Would you like to play again?  (yes or y to continue) : ")
