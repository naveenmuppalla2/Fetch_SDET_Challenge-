This type of problem can be solved using a divide and conquer approach. The goal is to reduce the number of possible
bars to check in each weighing.
Here's a step-by-step guide:

Label the Bars: Number the gold bars from 0 to 8 so that you can refer to them easily.

First Weighing (3 vs. 3):

Put three bars on the left side of the scale (e.g., bars 0, 1, and 2).
Put three bars on the right side of the scale (e.g., bars 3, 4, and 5).
Leave the remaining three bars out.
Now, you have three possible outcomes:

If the scale is balanced, the fake bar is among bars 6, 7, and 8.
If the left side is lighter, the fake bar is among bars 0, 1, or 2.
If the right side is lighter, the fake bar is among bars 3, 4, or 5.

Second Weighing (1 vs. 1):

Take the three remaining bars that weren't weighed in the first step.
Pick any two of them and place one on the left side and one on the right side of the scale.
Now, there are three possible outcomes:

If the scale is balanced, the fake bar is the one you didn't weigh.
If the left side is lighter, the fake bar is the one on the left.
If the right side is lighter, the fake bar is the one on the right.

This strategy ensures that you will find the fake gold bar in a maximum of two weighings. If the first weighing is
balanced, you can identify the fake bar in the second weighing. This approach minimizes the number of weighings
required.

Now, for test automation, We did create a script that simulates these steps on the provided website. We would need to
interact with the website's user interface to place the bars on the scale, record the results, and determine the fake
gold bar based on the outcomes. We used web automation tools Selenium with Java programming language to automate this
process.
