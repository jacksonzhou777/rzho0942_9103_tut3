# rzho0942_9103_tut3
My first repository for IDEA9103

This is my first local change to the repo!
1. 1 May - p5 project

# Quiz 8

## Part 1: Imaging Technique Inspiration

### Selected Technique: Dynamic Radial Ripple Propagation

For this week's quiz, I have identified the visual phenomenon of **water ripples** as my inspiration. I want to incorporate the **radial expansion** and **amplitude decay** of waves into my project. 

This technique is beneficial because it creates an organic and fluid visual language that effectively visualizes "impact" and "connection." By using ripples, I can transform abstract data from multiple mechanics—such as **Audio** levels, **Time-based** events, **Perlin Noise**, or **User Input**—into a tangible, meditative experience. This provides a reactive visual feedback system that scales naturally based on the intensity of the input.

#### Visual Inspiration Examples
![Natural ripple expansion 1](Images\ripple_1.jpg)

![Natural ripple expansion 2](Images\ripple_2.jpg)

> The images above illustrate how a single point of impact can influence the surrounding environment through wave propagation.

---

## Part 2: Coding Technique Exploration

### Selected Technique: Object-Oriented Programming (OOP) with Physics-based Mapping

To implement the imaging technique described in Part 1, I will use **Object-Oriented Programming (OOP)** in p5.js. Specifically, I will create a custom `Ripple` class to manage the lifecycle of each wave.

This coding technique helps achieve the desired effect by encapsulating properties like origin `(x, y)`, growth rate `radius`, and transparency `alpha` within each instance. To drive the mechanic, I will use:
* **User Input:** Mouse clicks trigger the ripple origin.
* **Audio:** Microphone levels map to the initial size.
* **Perlin Noise:** Adds organic distortion to the edges.
* **Time-based:** Timers reduce the alpha over time.

#### Implementation Preview
![Screenshot of the coding technique](Images\example_1.png)

#### Example Implementation and Code
You can find an example of this implementation via the links below:
[The Coding Train: Ripple Effect Sketch](https://openprocessing.org/sketch/2490490)
[p5.js Objects Reference](https://p5js.org/reference/)

```javascript
// Example of the logic I will use in my Ripple class
class Ripple {
  constructor(x, y) {
    this.x = x;
    this.y = y;
    this.r = 0;
    this.alpha = 255;
  }
}