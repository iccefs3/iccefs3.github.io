---
permalink: /sequences_instructions/
title: "Sequences Instructions"
author_profile: false
redirect_from: 
  - /sequences_instructions.html
---

# Quest Instructions

You are going to visit family friends! During this quest (4 puzzles in total), you will  bake a pie, ask for help, and take a long car trip to their house.

## Reminders & Hints:

1. A sprite is a character or object you can control with programming blocks.
1. Start each puzzle with the block, When Green Flag is Clicked  ![Start each puzzle with the block, When Green Flag is Clicked](/images/fs3/sequences_instructions/fs3_i_greenflag.png)
1. If your Parsons palette is grey (disabled ![parsons disabled](/images/fs3/sequences_instructions/parsons_grey.png)), you can use each enabled block multiple times.  If your Parsons palette is purple (enabled ![parsons enabled](/images/fs3/sequences_instructions/parsons_purple.png)), make sure to use each block in the palette at most once.
1. If you follow the instructions precisely, you can earn the highest score using the fewest moves for each puzzle.  This is your goal!  You might or might not receive various types of feedback and see blocks locked and unlocked to guide you as puzzles are solved.  Locked blocks can be unlocked by making correct moves with unlocked blocks.
1. You will not be able to submit until your solution is correct, or you’ve attempted two times the number of moves required to solve the puzzle. All blocks need to be connected to one another in order to run.
1. You might see a message similar to the one from Flash below.  Please select Allow.  This message applies to the virtual machine, and the storage used for necessary interaction tracing is small and harmless.

![flash storage message](/images/fs3/sequences_instructions/flash_storage.png)

## Warm up: Let’s Bake a Cake

In this puzzle, you are going to bake a pie for your friends.

First, you go to the location x=170, y=0, which is where the oven is located.
Second, you wait for 3 secs while the pie cooks.
Then, you change the costume of the sprite (next costume). This will turn the cake from unbaked, to baked!
Next, you take the pie to the location x=-150, y=0, which is where the table is.
Finally, you are happy with the result and say: “Your pie is ready!”

Remember to start each puzzle with the block, When Green Flag is Clicked

Number of blocks required to solve this puzzle: 6

The solution of this warm up phase is provided below (requires scrolling). Try to solve the puzzle yourself before comparing it with the solution.

Warm up Solution: 

![warm up solution](/images/fs3/sequences_instructions/warm-up_solution.png)

![when green flag clicked](/images/fs3/sequences_instructions/when_green_clicked.png): Don’t forget to use the when green flag clicked block to start the puzzle!
![go to x:170](/images/fs3/sequences_instructions/go_to.png): Use this block to go to a specified location of the oven.
![wait 3 seconds](/images/fs3/sequences_instructions/wait_3_seconds.png): This block allows the puzzle to wait for 3 seconds before proceeding to the next step. In this case, we have to wait 3 seconds for the pie to bake.
![next costume](/images/fs3/sequences_instructions/next_costume.png): This block changes the costume of the sprite. In our case, it changes the color of the pie after baking.
![go to x:-150](/images/fs3/sequences_instructions/go_to_2.png): Use this block to go to the new specified location when we take the pie out.
![say your pie is ready](/images/fs3/sequences_instructions/say.png): Use this to say things in the sprite. You can write attributes within the white rectangle. We use this block to say “Your pie is ready!” when the pie is ready.

## Puzzle 1: Asking for Help

You tried a slice of your pie and realized that you forgot to add sugar! In this puzzle, you will consult a recipe book to bake another pie for your friends.

First, you go to the recipe book at location x=-170, y=-30.
Second, you say one step of the recipe instruction (seen below) for 3 seconds (just to make sure you get it right this time!).
Third, you go to the mixing bowl to complete the task at location x=0, y=-30.
Fourth, you switch to next backdrop to reflect changes in the mixing bowl.
Then, make sure to wait for a second to see the changes. However, note that this only happens for the first two times.
There are three steps in the recipe book, so you go through the sequence above three times.

The recipe is as follows:
* Step1: Add flour and sugar.
* Step2: Add eggs and milk
* Step3: Mix

After you mix, you say “It’s time to bake”.

Number of blocks required to solve this puzzle: 16

## Puzzle 2: Are we there yet? - Part One

Your pie from the last puzzle was a success! You are really proud of yourself and decide to bring it to your friend’s house. You have decided to bring your younger friend Jasmine with you, who is rather inquisitive.

During the trip, she asks “Are we there yet?” for 5 seconds, then the car moves 50 steps.
This sequence happens **six times** until finally you say “we are there!”

Number of blocks required to solve this puzzle: 1450

## Puzzle 3: Are we there yet? - Part Two

To return home, we first need to turn the car around. We can turn around by pointing to -90 degrees.  Jasmine is still inquisitive, but this time she asks “Are we there yet?” for 3 seconds, then the car moves 130 steps to the left.  This sequence happens three times until finally you say “we are there!”

Number of blocks required to solve this puzzle: 9

## Puzzle 4: Playing Soccer

Your younger friend Jasmine is having a soccer match today! As a soccer star, she usually scores many goals during every game.

* First, she starts off the game at location x=-150, y =-50.
* Jasmine then thinks to herself: “I want to score three goals today!” for 2 seconds.
* She dribbles the ball for 300 steps and scores the first goal.
* Excitedly, she says: “Yay! One goal!” for 1 second.
* Then, she returns to the starting location x=-150, y =-50, and thinks to herself, “Two more!” for 2 seconds.
* She dribbles the ball for 300 steps again and scores the second goal.
* She yells: “Yay! Two goals!”
* After returning to the start location (x=-150, y =-50) again, she thinks, “One more!” for 2 seconds.
* Finally, she dribbles the ball for 300 steps and scores once again!
* At last,  Jasmine says: “Yay! Three goals! We win!”

Number of blocks required to solve this puzzle: 13

## Puzzle 5: The Brooklyn Bridge

To celebrate the victory with Jasmine, the two of you have decided to go on a boat ride and visit the Brooklyn Bridge at night.

1. To get on the boat, you go to location x=150, y = -100 and choose the boat of size 50%.
1. When the ride begins, Jasmine says: “We are 3 miles away!” for 2 seconds.
1. Then, the boat moves 80 steps to the left (-80 steps) and changes size by -10 as it sails further away from the dock.
1. Step two is then repeated two times for when you are 2 miles away and 1 mile away.
1. Finally, as you are closer to the Brooklyn bridge, you say: “We are here!”

Number of blocks required to solve this puzzle:13

# Puzzle 6: Saving For The Next Trip

You have had so much fun during the boat ride and want to start saving for the next big trip to Yellowstone. You plan to save for the next three months. Since you are a good baker now, you have decided to fund the trip through bake sales in addition to your regular salary.

To start, you put in $100 and think, “I have $100 for now” for 2 seconds.
Then, for the next two months, you do the following each month:

1. Add part of your salary to the fund and think, “Adding $100 from my salary!” for 2 seconds
1. Add part of your bake sale earnings to the fund and think, “Adding $50 from my bake sale!” for 2 seconds

After two months, your hard work has paid off, and you happily say: “Now we can go to Yellowstone!”

Number of blocks required to solve this puzzle: 7