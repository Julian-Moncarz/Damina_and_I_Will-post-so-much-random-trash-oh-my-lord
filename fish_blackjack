
#@title Code for the game - contains spoilers
import random as random
cards = [2, 3, 4, 5, 6, 7, 8, 9, 10, 10, 10, 10, 11]
def playgame():
  deck = []
  def deal():
    random.shuffle(deck)
    deck.remove(deck[0])
    return(deck[0])

  money = 100
  gameon = True
  print("You owe Mrs. Creditum Selachimorpha 1000 shells. You have decided to make back the cash with your skill at blackjack.")
  print("Earn 1000 shells and stay off Mrs. Selachimorpha's menu. Lose all your funds and...")
  print("Well, just don't go broke!!")
  while money > 0 and money <1000:
    gameon = True
    while gameon == True:
      print(f"You have {money} shells")
      i = 0
      deck = []
      while i<4:
        for rank in cards:
          card = rank
          deck.append(card)
          i = i+1
      bet = input('Place your bet!')
      patience = 3
      while not bet.isnumeric() and gameon:
        bet = input("Please bet a NUMBER, you stupid fucking shrimp!!: ")
        if patience > 0:
          patience -= 1
        if patience == 0:
          print("That's IT. Little fuckin' shrimp thinks they can screw with the the sharks...")
          print("Mr. Squalus! This little shrimp punk is ON THE MENU!")
          print("...")
          print("CHOMP!")
          print("GAME OVER.")

  #nothing stops you from betting an amount you don't have, eg 999,999,999,999,999
  #if you lose, you'll be devoured, but it's an easy way to win the game in 1 turn
  #I'm leaving it in as a reward for anyone smart enough to find it


      hand = deal()+deal()
      showcard = deal()
      dealer = deal()+showcard
      if hand == 22:
        hand = 12
      if gameon == True:
        print(f"Your hand is {hand}")
      if hand == 21:
        print("Blackjack!")
        gameon = False
        money = money + float(bet)
      if gameon == True:
        print(f"The dealer's face up card is a {showcard}")
      choice = "whatever placeholder im too lazy too deal with the error I dont want to indent anything blah blah blahhhh AHHHHH AHHHHH AAAAAAAHHHHHHHHHHH... CHOMP!"
      if gameon == True:
        choice = input("Would you like to hit or stay?")
      while choice == "hit" and gameon == True:
        hand = hand+deal()
        print(f"Your hand is {hand}")
        if hand > 21 and gameon == True:
          money = money - float(bet)
          gameon = False
          print('Fuckin BUST, Suca!')
        elif gameon == True:
          choice = input("Would you like to hit or stay?")
      if gameon == True:
       print(f"The dealer's hand is {dealer}")
      while dealer < 14 and gameon == True:
        print("The dealer has less then 14. They must draw")
        dealer = dealer+deal()
        print(f"The dealer draws up to {dealer}")
      if dealer > 21 and gameon == True:
        print("The dealer goes bust! You win!")
        money = money+float(bet)
        gameon = False
      if dealer > hand and gameon == True:
        print("The dealer has the better hand. You lose.")
        money = money-float(bet)
        gameon = False
      elif hand>dealer and gameon == True:
        print("You have the better hand. You win!")
        money = money+float(bet)
        gameon = False
      elif hand == dealer and gameon == True:
        print("You and the dealer tie.")
        gameon = False
  if money <= 0:
    print("YOU HAVE ZERO MUNEEZ...")
    print("Dun. Dun.")
    print("Dun dun.")
    print("Dun dun.")
    print("Dun dun.")
    print("Dun dun dun dun dun dun dun...")
    print("CHOMP!")
    print("GAME OVER.")
  elif money >= 1000 and money <= 100000:
    print(f"You have {money} shells")
    print("Well done, shrimp! You payed off your debt! Mrs. Selachimorpha will take the extra as intrest...")
    print("And just hope she's not feeling HUNGRY.")
    print("You have 0 shells")
  elif money > 1000000:
    print(f"You have {money} shells")
    print('Your the biggest fish in town')
    easter = input('Since you so rich... would you like to pay to have Mrs. Selachimorpha... removed?')
    if easter == 'yes' or easter == "Yes":
      money = money - money/4
      print(f"You have {money} shells")
      print("The very next day Mrs. Selachimorpha somehow swallows an oxygen tank")
      print("And someone shoots it...")
      print("KABOOM!!")
      print("Mrs. Selachimorpha's explodeded corpse lies at your fins.")
      print("YOU WIN.")
    else:
      print("You pay back your debt.")
      print("A few years pass, and Mrs. Selachimorpha is feeling...")
      print("HUNGRY")
      print("...")
      print("CHOMP!")
playgame()
