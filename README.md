# moonimport matplotlib.pyplot as plt
import numpy as np

def draw_moon():
    # Create a figure and axis
    fig, ax = plt.subplots()

    # Create a circle representing the moon
    moon = plt.Circle((0.5, 0.5), 0.4, color='lightgray')

    # Create a smaller circle to simulate a shadow (like a crescent moon)
    shadow = plt.Circle((0.7, 0.5), 0.35, color='black')

    # Add the moon and shadow to the plot
    ax.add_artist(moon)
    ax.add_artist(shadow)

    # Set the aspect ratio to be equal
    ax.set_aspect('equal')

    # Remove axes
    plt.axis('off')

    # Show the plot
    plt.show()

# Draw the moon
draw_moon()
