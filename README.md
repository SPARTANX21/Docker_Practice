# 🐳 Docker Practice Project

Welcome to the **Docker Practice** repository — a hands-on beginner-friendly project designed to help you learn the fundamentals of Docker by containerizing a simple Python-based BMI (Body Mass Index) calculator.

Whether you're just starting with containers or brushing up your Docker skills, this project provides a clean, guided learning experience.

---

## 📁 Project Structure

Docker_Practice/

│
├── bmi.py # A Python script for calculating BMI

├── Dockerfile # Dockerfile to containerize the Python script

├── Docker commands .txt # A reference file for basic Docker commands

└── README.md # This file


---

## 📌 Objective

This project will teach you:

- How to write a **Dockerfile**
- How to **containerize** a Python app
- How to **build and run Docker images**
- How to run interactive containers
- Basic Docker CLI commands

---

## 🧠 About `bmi.py`

This Python script calculates Body Mass Index:

- Takes **weight** (kg) and **height** (m) as input
- Computes: `BMI = weight / (height * height)`
- Classifies result:
  - Underweight
  - Normal weight
  - Overweight
  - Obese

---

## 🐋 Dockerfile Overview

Your `Dockerfile` includes:

1. **Base Image** – e.g. `python:3.10`
2. **Working Directory** setup
3. **Copy Command** – moves `bmi.py` into container
4. **Run Instructions** – for setup (if needed)
5. **CMD** – runs the BMI calculator interactively

---

## 🚀 How to Use

### 1. Clone the Repository

```bash
git clone https://github.com/SPARTANX21/Docker_Practice.git
cd Docker_Practice

docker build -t docker-bmi-app .

docker run -it docker-bmi-app
The -it flag makes the container interactive so you can input values.
```

### 📘 Docker Commands Cheat Sheet
Useful commands from Docker commands .txt:

Command	Description

- docker build -t name .	Build Docker image
- docker images	List all images
- docker run -it name	Run container interactively
- docker ps	Show running containers
- docker stop <id>	Stop a container
- docker rm <id>	Remove a container
- docker rmi <id>	Remove an image

### 🎯 Learning Goals

✅ Understand Docker fundamentals

✅ Create your first container

✅ Use Docker CLI with confidence

✅ Learn image creation and containerization

✅ Practice running interactive scripts in Docker


### Ideas to Expand

- You can take this further by:

- Converting to a Flask API or Streamlit UI

- Publishing the image to DockerHub

- Adding input validation

- Writing unit tests

## Feedback
Feel free to open issues or suggestions! Happy to collaborate and grow this practice repo. 🌱



