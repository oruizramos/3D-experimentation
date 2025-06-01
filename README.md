# Check it live!

https://3d-physics-experiment.netlify.app/

# Physics Experimentation

- Interactive 3D Physics Simulation with Three.js and Rapier

# Overview

- This is a simple browser-based 3D simulation that showcases real-time physics interactions using Three.js for rendering and Rapier for physics computations. Users can interact with a dynamic environment where multiple objects respond to physics laws, and a custom 3D cursor enhances the immersive experience.

# Features

- 3D Rendering: Utilizes Three.js to render a visually appealing 3D scene.

- Physics Engine: Implements Rapier for accurate and efficient physics simulations.

- Custom Cursor: Replaces the default cursor with a 3D model (Spaceship.glb) that follows mouse movements.

- Interactive Objects: Loads multiple instances of a 3D model (Planet1.glb) that interact with the environment and each other.

- Orbit Controls: Allows users to navigate the scene using mouse controls.

- Responsive Design: Adjusts to different screen sizes and window resizes.

# Tech Stack

- Three.js: JavaScript 3D library for rendering.

- Rapier: Rust-based physics engine compiled to WebAssembly for performance.

- GLTFLoader: Loads .glb 3D models into the scene.

- OrbitControls: Enables intuitive camera controls.

- JavaScript (ES6 Modules): Modular code structure for maintainability.

📁 Project Structure
nginx
Copy
Edit
Physics Experiment/
├── Planet1.glb         # 3D model used for dynamic objects
├── Spaceship.glb       # 3D model used as a custom cursor
├── getBodies.js        # Module to create physics bodies
├── index.html          # Main HTML file
├── index.js            # Main JavaScript file
└── README.md           # Project documentation

# Getting Started

- Prerequisites

To run the project locally, you need to serve it over a local web server due to browser restrictions on loading local files.

Steps

Clone the Repository

git clone https://github.com/yourusername/physics-experiment.git
cd physics-experiment
Start a Local Server

You can use Python's built-in server:

For Python 3:

python -m http.server

For Python 2:

python -m SimpleHTTPServer

Alternatively, use any other local server of your choice.

Open in Browser

Navigate to http://localhost:8000 (or the port specified by your server) in your web browser to view the simulation.

# How It Works

- Scene Initialization

- Sets up the Three.js scene, camera, and renderer.

- Adds lighting to illuminate the scene.

- Physics World Setup

- Initializes the Rapier physics world with gravity.

- Creates a static ground collider to serve as the floor.

# Model Loading

- Loads Planet1.glb and creates multiple instances with physics bodies.

- Loads Spaceship.glb to replace the default cursor with a 3D model.

- Mouse Interaction

- Captures mouse movements and updates the position of the custom cursor.

- Uses raycasting to determine the intersection point on the floor.

- Animation Loop

- Updates physics simulations.

- Renders the scene continuously.

- Updates object positions based on physics calculations.


# License

This project is licensed under the MIT License. See the LICENSE file for details.





