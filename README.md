# Snake-Water-Gun-Game
This is a simple snake water gun game, code is written in Python.
<br>
Author - Khubaib Husain

import random

Computer = random.choice([-1, 0, 1])
YouString = input("Enter your choice (S,W,G) ( CAPITAL LETTERS ONLY ): ")
YouDict = {"S": 1, "W": -1, "G": 0}
You = YouDict[YouString]
ReversedDict = {1: "Snake", -1: "Water", 0: "Gun"}

if Computer == You:
    print(
        f"It's a Draw! because computer chose {ReversedDict[Computer]} and you also chose {ReversedDict[You]} (Both have chosen same)"
    )

elif Computer == -1 and You == 1:
    print(
        f"You Win! because computer chose {ReversedDict[Computer]} and you chose {ReversedDict[You]} "
    )

elif Computer == 1 and You == -1:
    print(
        f"You Lose! because computer chose {ReversedDict[Computer]} and you chose {ReversedDict[You]} "
    )

elif Computer == -1 and You == 0:
    print(
        f"You Lose! because computer chose {ReversedDict[Computer]} and you chose {ReversedDict[You]} "
    )

elif Computer == 1 and You == 0:
    print(
        f"You Win! because computer chose {ReversedDict[Computer]} and you chose {ReversedDict[You]} "
    )

elif Computer == 0 and You == -1:
    print(
        f"You Lose! because computer chose {ReversedDict[Computer]} and you chose {ReversedDict[You]} "
    )

elif Computer == 0 and You == 1:
    print(
        f"You Win! because computer chose {ReversedDict[Computer]} and you chose {ReversedDict[You]} "
    )
