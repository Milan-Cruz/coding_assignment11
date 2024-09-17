```markdown
# Coding Assignment 11

This project demonstrates a React application inside a Docker container that displays a `<h1>` tag with the text "Codin 1". Follow the steps below to recreate the setup locally.

## Developed by Milan Cruz

## Prerequisites

Before cloning and running the project, make sure the following software is installed on your Windows machine:

1. **Node.js** (version 14.x or later)
2. **Yarn** (version 1.22 or later)
3. **Docker Desktop** (with WSL2 or Hyper-V backend)
4. **Git** (version 2.x or later)

You can verify the installations with the following PowerShell or Command Prompt commands:

node --version
yarn --version
docker --version
git --version

## Instructions for Windows Users

### Step 1: Clone this GitHub Repository

In **PowerShell** or **Command Prompt**, run the following commands:

```bash
git clone https://github.com/Milan-Cruz/coding_assignment11.git
cd coding_assignment11
```

### Step 2: Install Dependencies

```bash
yarn install
```

### Step 3: (Optional) Run the Application Without Docker

If you'd like to run the application without Docker, use this command:

```bash
yarn start
```

This will start the development server on [http://localhost:3000](http://localhost:3000).

### Step 4: Build the Docker Image

To build the Docker image, use the following command:

```bash
docker build -t cruz_milan_coding_assignment11 .
```

### Step 5: Run the Docker Container

To run the Docker container, use this command:

```bash
docker run -d -p 7775:7775 --name cruz_milan_coding_assignment11 cruz_milan_coding_assignment11
```

### Step 6: Access the Application

Once the container is running, open a browser and navigate to [http://localhost:7775](http://localhost:7775) to view the application.

### Step 7: Start the Docker Container in Subsequent Runs

If you stop the container and want to start it again in future runs, you can use the following command to restart the container without rebuilding it:

```bash
docker start cruz_milan_coding_assignment11
```

## Stopping and Removing the Docker Container

If you need to stop or remove the running container, use the following commands:

```bash
docker stop cruz_milan_coding_assignment11
docker rm cruz_milan_coding_assignment11
```

## License

This project is licensed under the MIT License.
```
Last Addition:
- Step 7: I added a section explaining how to start the Docker container in subsequent runs using the `docker start` command. This will allow users to restart the container without having to rebuild it each time.