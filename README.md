# Visualizing Frequency Components of a 3D Curve with Discrete Fourier Transform

![](https://cdn.glitch.com/9b7da1a6-c1c0-4233-a217-94e0d5c696a8%2FDFT_Screenshot.PNG.jpg?v=1599416645984)

View on desktop, mobile, or VR: [DFT.Glitch.me](https://dft.glitch.me/)

WASD to move.

Explanation:
The 3D curve was originally drawn in Tilt Brush (rough tracing of a dune buggy). The curve was then exported from Tilt Brush as a series of X, Y, Z coordinates over time.

![](https://cdn.glitch.com/9b7da1a6-c1c0-4233-a217-94e0d5c696a8%2FTBCar.png?v=1599417341191)

I run a DFT over each coordinate time-series to produce frequency components for each dimension. These frequency components are visualized directly as a series of rotating vectors added tip to tail, inspired by [3blue1brown](https://bit.ly/2kfCcfI). Summing the results of all vectors for each dimension produces 3D coordinates over time, which reconstructs the original 3D curve.
![](https://cdn.glitch.com/9b7da1a6-c1c0-4233-a217-94e0d5c696a8%2FDFT_Arrows.jpg?v=1599417820125)

It is interesting to play with the number and filtering of the frequency components to see the visual effects (3D smoothing, sharpening) and rendering performance impact.

Developed in Three.js / A-Frame

Credit Daniel Shiffman for DFT code starting point: [link](https://editor.p5js.org/codingtrain/sketches/RfrZibjfL)
