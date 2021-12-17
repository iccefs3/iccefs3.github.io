---
permalink: /conditionals_instructions/
title: "Conditionals Instructions"
author_profile: false
redirect_from: 
  - /instructions.html
  - /conditionals_instructions.html
  - /instructions/
---
## Quest Instructions:

You are off for a vacation! During this quest (4 puzzles in total), you will visit a casino, shop for supplies, go sailing, and scuba dive.

## Reminders & Hints:

1. A **sprite** is a character or object you can control with programming blocks.
1. If your Parsons palette is grey (disabled ![disabled](/images/conditionals_instructions/parsons_disabled.png)), you can use each enabled block multiple times.  If your Parsons palette is purple (enabled ![enabled](/images/conditionals_instructions/parsons_enabled.png)), make sure to use each block in the palette at most once.
1. If you follow the instructions precisely, you can earn the **highest score** using the **fewest moves** for each puzzle. This is your goal!  Choose carefully before moving each block from the palette.
1. You will not be able to submit your solution until it is correct, or you have attempted twice the number of moves required to solve the puzzle successfully.

## Important Boolean Blocks:

Picking random number and compare blocks:
![pick random](/images/conditionals_instructions/pick_random.png)
![equals](/images/conditionals_instructions/equals.png)
![less than](/images/conditionals_instructions/less_than.png)

![pick random equals](/images/conditionals_instructions/pick_random_equals.png)
![pick random less than](/images/conditionals_instructions/pick_random_less_than.png)

Touching color block:
![touching color](/images/conditionals_instructions/touching_color_green.png)

We will provide these blocks to you in the instructions when needed.  They will not contribute to your total move count.

## Warm up puzzle: At the casino

During your vacation, you go to the casino with your friend Kala and decide to play roulette! You choose to play by color. There are two options, red and black. In this puzzle: 1=red and 2=black.


First, you say: "I am choosing red.”

Then, you pick a random number from 1 to 2, using the pick random and compare blocks. 
![pick random equals](/images/conditionals_instructions/pick_random_equals.png)


If that number equals 1, then your friend Kala says “It’s red! You win!”.

Else, she says “It’s black, you lose!”

Number of blocks required to solve this puzzle: 7

The solution of this warm up phase is provided below (requires scrolling). Try to solve the puzzle yourself before comparing it with the solution.









































Warm up Solution:

![warm up solution](/images/conditionals_instructions/warm_up_solution.png)

![when start clicked](/images/conditionals_instructions/when_start_clicked.png)：Don’t forget to use the when green flag clicked block to start the puzzle!

![casino choice](/images/conditionals_instructions/casino_choice.png)：Use this to say things in the sprite. You can write attributes within the white rectangle.

![if else](/images/conditionals_instructions/if_else.png)：This is a if-else conditional block. If the condition in the diamond shaped space is satisfied, you go into the if condition. However, if the diamond shaped condition is not met, then you enter the else condition.

![pick random filled](/images/conditionals_instructions/pick_random_filled.png): This block lets you pick a random number. In this case, it's either 1 or 2. 1 means the color red, and 2 means the color black on the roulette wheel.

![pick random equals filled](/images/conditionals_instructions/pick_random_equals_filled.png): This block compares two values and allows you to embed other blocks, such as pick random. As a result, you can choose a random number and evaluate if the random number equals 1. If the random number=1, then it enters the if condition. If the random number=2, then it enters the else condition.

![win condition](/images/conditionals_instructions/win_condition.png): This is the statement in the if condition. This means that if the random number=1, the sprite will say “It’s red! You win!”.

![lose condition](/images/conditionals_instructions/lose_condition.png): This is the statement in the else condition. This means that if the random number=2, the sprite will say “It’s black, you lose!!!”.

## First puzzle: Shopping for supplies

The casino was a huge success for both you and Kala! You have decided to use the money you won and go sailing. However, you need to go to the sailing store to get supplies first.


First, you go to location x=130, y=50, which is your starting location. You remembered that you need to go to your car to get cash before going to the store.


Therefore, if you are touching color grey (color of the road): ![touching color grey](/images/conditionals_instructions/touching_color_grey.png)

        You move 180 steps to find your car.

        Then, you say “Here is my car! Let me get some money! “ for 2 seconds.

        You then wait for 3 sec to find cash in the car!

Now, if you are touching color red (color of the car):![touching color red](/images/conditionals_instructions/touching_color_red.png)

        You go to location x=240, y=230, which is where the sailing store is.

        Once you get there, you say “Here is the sailing store!” for 2 seconds.

Number of blocks required to solve this puzzle: 11
































## Second puzzle: When to sail today?

Now that you have gotten your supplies, you are ready to sail with Kala! However, you want to check the weather to decide if you should sail during the day or at night.


Your boat starts at location x=0, y=-25.

You then say: “Let me check the weather, when should we sail today?”

Now, you pick a random number from 1 to 2. 1 means sailing during daytime and 2 means sailing during night time.

![pick random equals](/images/conditionals_instructions/pick_random_equals.png)

If the random number equals to 1, then:

        You switch the background (backdrop) to “daytime”.

        You then think to yourself: “I should sail during the day!”

        And you sail 200 steps to begin your sailing journey.

Else:

        You switch the background (backdrop) to “night time”.

        You then think to yourself: “I should sail at night today!”

        You then happily sail 200 steps to begin your sailing journey.

Number of blocks required to solve this puzzle: 12



















## Third puzzle: Finding gems in the ocean

Your friend Kala tells you she has heard of long-lost gems at the bottom of this part of the ocean. Since you still have lots of money left from the casino, you have decided to go on a scuba dive trip to try to find all those gems!


You first jump into the ocean at location x=-20, y=10.


We will use a random process to determine whether your search will be successful. Therefore, you pick a random number between 1 and 10.

![pick random less than](/images/conditionals_instructions/pick_random_less_than.png)

If the number is smaller than 5:

        You swim 100 steps.  All of the sudden you see the gems!

        Excitedly, you say: “I found the gems!” for 2 seconds.

        You then go to location x=20 and y=-90 to retrieve the gems!

Else:

        You still swim 100 steps.

        However, you say: “Oops, I didn’t find anything”,

        Frustratedly, you then swim another 300 steps.

Number of blocks required to solve this puzzle: 11