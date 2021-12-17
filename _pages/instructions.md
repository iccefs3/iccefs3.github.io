---
permalink: /instructions/
title: "Instructions"
author_profile: false
redirect_from: 
  - /sequences_instructions.html
  - /instructions.html
---
Quest Instructions
------
You are going to visit family friends! During this quest (4 puzzles in total), you will  bake a pie, ask for help, and take a long car trip to their house.

Reminders & Hints
------
A sprite is a character or object you can control with programming blocks.

If you follow the instructions precisely, you can earn the **highest score** using the **fewest moves** for each puzzle. This is your goal!  Choose carefully before moving each block from the palette.

Warm up: Let’s Bake a Cake
------
In this puzzle, you are going to bake a pie for your friends.

1. First, you go to the location (x= 170, y=0), which is where the oven is located.
1. Second, you wait for 3 secs while the pie cooks.
1. Then, you change the costume of the sprite (next costume). This will turn the cake from unbaked, to baked!
1. Next, you take the pie to the location (X=-150, y=0), which is where the table is.
1. Finally, you are happy with the result and say: “Your pie is ready!”

Number of blocks required to solve this puzzle: 6

The solution of this warm up phase is provided below. Try to solve the puzzle yourself before comparing it with the solution.

Warm up Solution:
{% include image-gallery.html folder="/images/sequences_instructions/i0" %}
![](/images/sequences_instructions/i0/fs1_c1_i0.png)
* Don’t forget to use the when green flag clicked block to start the puzzle!
* Use this block to go to a specified location of the oven.
* This block allows the puzzle to wait for 3 seconds before proceeding to the next step. In this case, we have to wait 3 seconds for the pie to bake.
* This block changes the costume of the sprite. In our case, it changes the color of the pie after baking.
* Use this block to go to the new specified location when we take the pie out.
* Use this to say things in the sprite. You can write attributes within the white rectangle. We use this block to say “Your pie is ready!” when the pie is ready.

Puzzle 1: Asking for Help
------
You tried a slice of your pie and realized that you forgot to add sugar! In this puzzle, you will consult a recipe book to bake another pie for your friends.

1. First, you go to the recipe book at location x:-170, y:-30.
1. Second, you say one step of the recipe instruction (seen below) for 3 seconds (just to make sure you get it right this time!).
1. Third, you go to the mixing bowl to complete the task at location x:0, y:-30.
1. Fourth, you switch to next backdrop to reflect changes in the mixing bowl.
1. Then, make sure to wait for a second to see the changes. However, note that this only happens for the first two times.
1. There are three steps in the recipe book, so you go through the sequence above three times.
    The recipe is as follows:
    1. Step1: Add flour and sugar.
    1. Step2: Add eggs and milk
    1. Step3: Mix
1. After you mix, you say “It’s time to bake”.

Number of blocks required to solve this puzzle: 16
{% include image-gallery.html folder="/images/sequences_instructions/i1" %}
![](/images/sequences_instructions/i1/fs1_c1_i1.png)

Puzzle 2: Are we there yet? - Part One
------
Your pie from the last puzzle was a success! You are really proud of yourself and decide to bring it to your friend’s house. You have decided to bring your younger friend Jasmine with you, who is rather inquisitive.

During the trip, she asks “Are we there yet?” for 5 seconds, then the car moves 50 steps.

This sequence happens six times until finally you say “we are there!”

Number of blocks required to solve this puzzle: 14
{% include image-gallery.html folder="/images/sequences_instructions/i2" %}
![](/images/sequences_instructions/i2/fs1_c1_i2.png)

Puzzle 3: Are we there yet? - Part Two
------
Now, is there a better way to represent the previous scenario? Do we need to use new blocks everytime Jasmine repeats the same question? Probably not. Now, the challenge is to find a simpler puzzle construction to solve the previous problem. You are allowed to use each block only once!

To refresh your mind, the instruction for the puzzle is:

    “Your pie from the last puzzle was a success! You are really proud of yourself and decide to bring it to your friend’s house.
    You have decided to bring your younger friend Jasmine with you, who is rather inquisitive.

During the trip, she asks “Are we there yet?” for 5 seconds every time the car moves 50 steps.

She repeats six times until finally you say “we are there!”

Number of blocks required to solve this puzzle: 5
{% include image-gallery.html folder="/images/sequences_instructions/i3" %}
![](/images/sequences_instructions/i3/fs1_c1_i3.png)