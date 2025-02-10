# Torred-schwann

import turtle as t
import colorsys as cs

import turtle as t
import colorsys as cs

# Setup turtle
t.speed(80)  # Set high speed for fast drawing
t.tracer(10)  # Reduce update delay for smoother animation
t.width(2)  # Set pen width
t.bgcolor('black')  # Set background color

# Main drawing loop
for j in range(25):
    for i in range(15):
        # Set color based on HSV color model
        t.color(cs.hsv_to_rgb(i / 15, j / 25, 1))

        # Draw pattern
        t.right(90)
        t.circle(200 - j * 4, 90)
        t.left(90)
        t.circle(200 - j * 4, 90)
        t.right(180)
        t.circle(50, 24)

# Finalize
t.hideturtle()
t.done()
