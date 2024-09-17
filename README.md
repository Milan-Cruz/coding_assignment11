# Coding Assignment 11

This project demonstrates a React application inside a Docker container that displays a <h1> tag with the text "Codin 1". Follow the steps below to recreate the setup locally.

## Developed by Milan Cruz

## Prerequisites

Before cloning and running the project, make sure the following software is installed on your machine:

1. **Node.js** (version 14.x or later)
2. **Yarn** (version 1.22 or later)
3. **Docker** (version 20.x or later)
4. **Git** (version 2.x or later)

You can verify the installations with the following commands:

bash
node --version
yarn --version
docker --version
git --version


## Instructions

### Step 1: Clone this GitHub Repository:

bash
git clone https://github.com/Milan-Cruz/coding_assignment11.git
cd coding_assignment11


### Step 2: Install Dependencies:

bash
yarn install


### Step 3: (Optional) Run the Application Without Docker:

If you'd like to run the application without Docker, use this command:

bash
yarn start


### Step 4: Build the Docker Image:

bash
docker build -t cruz_milan_coding_assignment11 .


### Step 5: Run the Docker Container:

bash
docker run -d -p 7775:7775 --name cruz_milan_coding_assignment11 cruz_milan_coding_assignment11


### Step 6: Access the Application:

The application will be available at [http://localhost:7775](http://localhost:7775).

## License

This project is licensed under the MIT License.