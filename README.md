# Webpage Animation Project
## 3D GSAP Scroll Animations

This repository contains the source code for a webpage animation project. The animation is built using GSAP (GreenSock Animation Platform) and the ScrollTrigger plugin to create an engaging and interactive user experience.

## Getting Started

To get started with this project, follow these instructions:

### Prerequisites

Make sure you have the following software installed on your machine:

- Node.js
- npm (Node Package Manager)

### Installation

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/your-username/your-repo.git

Certainly! Here's a template for a README.md file for your GitHub repository, including the explanation of the JavaScript code:

```markdown
# Webpage Animation Project

This repository contains the source code for a webpage animation project. The animation is built using GSAP (GreenSock Animation Platform) and the ScrollTrigger plugin to create an engaging and interactive user experience.

## Getting Started

To get started with this project, follow these instructions:

### Prerequisites

Make sure you have the following software installed on your machine:

- Node.js
- npm (Node Package Manager)

### Installation

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/your-username/your-repo.git
   ```

2. Navigate to the project directory:

   ```bash
   cd your-repo
   ```

3. Install the required dependencies:

   ```bash
   npm install
   ```

4. Open the `index.html` file in a web browser to view the animation.

## Animated Section

This section of the webpage features animations triggered by scrolling.

### JavaScript Code Explanation

The animation is managed by the `script.js` file. Let's break down the key parts of the code:

```javascript
var tl = gsap.timeline({
  scrollTrigger: {
    trigger: ".part-2",
    start: "20% 50%",
    end: "100% 59%",
    scrub: 2,
    pin: true,
  },
});

tl.to(
  "#image-anim-2",
  {
    opacity: 0,
  },
  "a"
).to(
  ".image-anim",
  {
    rotateX: "0deg",
    top: "-10vh",
  },
  "a"
);
```

#### 1. Timeline Initialization

A GSAP timeline is created to manage the animations over time. The `scrollTrigger` option is configured to define how the animation responds to scrolling.

#### 2. ScrollTrigger Options

- `trigger: ".part-2"`: The animation is triggered by the element with the class `part-2`.
- `start: "20% 50%"`: The animation starts when the trigger element is 20% from the top and 50% from the left.
- `end: "100% 59%"`: The animation ends when the trigger element is 100% from the top and 59% from the left.
- `scrub: 2`: Enables smooth scrolling-based animation with a scrubbing effect.
- `pin: true`: Pins the trigger element during the animation.

#### 3. Tween Animations

Two animations are defined within the timeline, triggered by scrolling through the specified section (`part-2`), providing a visually appealing and interactive experience.

Feel free to explore and modify the code to suit your needs!
```

Replace "your-username" and "your-repo" with your GitHub username and repository name, respectively. This README.md provides users with an overview of the project, instructions on getting started, and a detailed explanation of the JavaScript code used for the animation.
