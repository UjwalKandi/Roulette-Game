# Roulette-Game <img src="https://media.giphy.com/media/26uflBhaGt5lQsaCA/source.gif?cid=ecf05e47f308ctagp662symv4glxsp55d5dydl3hmcp5e0oi&rid=source.gif&ct=g" width="50">
This program simulates a game of roulette. In roulette, a wheel spins and yields a number between 1 and 49 when a ball drops into a numbered slot. The initial amount is monitored throughout the game and will be reminded to the player after each guess. If the amount goes zero, then the game ends.


```python
from random import randint

totalAmount=1000                            #total amount invested 

while totalAmount > 0:
    print("Welcome !!!\nYou have", totalAmount,"€. Good Luck !!\n_________________________________")
    selectedNumber=int(input("\nOn which number do you want to bet ?"))
    
    x=0
    x=selectNumber
    
    if x < 0 or x > 49:
        print("You have to bet a number between 0 and 49")
    
    bettingAmount=int(input("How much do you want to bet on this number?"))
    numberOutput = randint(0, 49) # line to use to generate a random number between 0 and 49
    print("\nThe number output is",numberOutput)
    
    if numberOutput == selectedNumber:
        print("You Win!!!\n_________________________________")
    else:
        print("Sorry but you lost, try again !")
        totalAmount-=bettingAmount
        print("\nYou now have",totalAmount,"€ left\n_________________________________")
        
if totalAmount==0:
    print("Sorry but you don't have enough money to continue !\nThe game is now ending !")
```

```
Welcome !!!
You have 1000 €. Good Luck !!
_________________________________

On which number do you want to bet ?5
How much do you want to bet on this number?500

The number output is 9
Sorry but you lost, try again !

You now have 500 € left
_________________________________
Welcome !!!
You have 500 €. Good Luck !!
_________________________________

On which number do you want to bet ?5
How much do you want to bet on this number?500

The number output is 36
Sorry but you lost, try again !

You now have 0 € left
_________________________________
Sorry but you don't have enough money to continue !
The game is now ending !
```
