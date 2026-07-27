# Real-Time-Animated-Sine-Wave-Visualization

A Python script that generates a dynamic, real-time scrolling sine wave animation using matplotlib and NumPy.

---

## Features

* **Scrolling Viewport**: Maintains a fixed window width ($4\pi$) that dynamically slides as new data points are generated.
* **Buffer Management**: Retains a rolling window of the last 200 data points for smooth performance.
* **Optimized Rendering**: Uses blit=True with matplotlib.animation.FuncAnimation for efficient, high-frame-rate rendering.
* **GIF Export Support**: Includes commented code to export the animation as an animated GIF using Pillow.

## Prerequisites
Ensure you have Python installed along with the required dependencies:

pip install matplotlib numpy pillow

## How to Run

Execute the script using Python:

python main.py

## Saving as a GIF

To export the animation as a .gif file, uncomment the following line before running the script:

ani.save('sine_wave.gif', writer='pillow', fps=30)
