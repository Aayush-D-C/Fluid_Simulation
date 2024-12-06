<h1>🌊 Particle Simulation Project</h1>
📝 Overview
This is a simple 2D particle simulation implemented in C++ using graphics.h, demonstrating basic physics principles like gravity, friction, and particle movement.
✨ Features

🔢 Particle system with 100 particles
🌍 Gravity and friction simulation
🏀 Particle bouncing off screen boundaries
🎲 Randomized initial particle positions and velocities

🛠 Prerequisites

💻 C++ Compiler (GCC/G++)
🖼 Graphics library (graphics.h)
🏗 CMake
🖼️ ImageMagick (for GIF generation)

📦 Dependencies

graphics.h library
CMake
ImageMagick

💾 Installation
🐧 Ubuntu/Debian
bashCopysudo apt-get update
sudo apt-get install build-essential cmake libx11-dev imagemagick
🍎 macOS (with Homebrew)
bashCopybrew install cmake imagemagick
🚀 Building the Project
Using CMake

🔽 Clone the repository

bashCopygit clone https://github.com/yourusername/particle-simulation.git
cd particle-simulation

📁 Create build directory

bashCopymkdir build
cd build

🔨 Generate Makefile and build

bashCopycmake ..
make
🎥 Generating Simulation GIF
🎬 Recording Method

Install ffmpeg or use ImageMagick
Run the simulation and record screen

bashCopy# Example using ffmpeg
ffmpeg -f x11grab -s 640x480 -i :0.0 output.gif
🖼 Alternative GIF Generation
bashCopy# Using ImageMagick to convert frames
convert -delay 20 -loop 0 frame*.png simulation.gif
🕹 Running the Simulation
bashCopy./particle_simulation
🔧 Customization
Edit the following macros in the source code to modify simulation:

NUM_PARTICLES: Number of particles
PARTICLE_SIZE: Size of each particle
GRAVITY: Gravitational acceleration
FRICTION: Velocity reduction factor

📋 TODO

 Add more physics interactions
 Implement color variations
 Create more complex particle behaviors