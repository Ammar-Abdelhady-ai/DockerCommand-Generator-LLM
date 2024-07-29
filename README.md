# DockerCommand-Generator-LLM
 Unsloth/Mistral7B-Docker-Command-Generator

# Fine-Tune Mistral-7B-v0.1 Model using Unsloth on DockerNLCommands Dataset

## Project Overview

This project involves fine-tuning the Mistral-7B-v0.1 model using the Unsloth library on the DockerNLCommands dataset. The goal is to develop a Large Language Model (LLM) that can generate Docker commands based on natural language input. This means you can input a description of the task you want to perform, and the model will generate the corresponding Docker command.

## Key Features

- **Model:** Mistral-7B-v0.1
- **Dataset:** DockerNLCommands
- **Fine-Tuning Library:** Unsloth

Unsloth is an optimized library designed for fine-tuning Large Language Models. It significantly boosts training speed, reduces memory usage, and increases overall efficiency, saving a substantial amount of training time.

## Project Goals

- Create an LLM that can write Docker commands based on natural language descriptions.
- Optimize the fine-tuning process to ensure efficient and seamless integration of new data.
- Achieve high performance and accuracy in generating correct Docker commands.

## Career Objective

My career goal is to become a leading expert in AI model optimization and deployment, ensuring efficient and seamless integration of new data to continuously improve model performance.

## Getting Started

### Prerequisites

- Docker
- Python 3.8+
- Unsloth library
- Mistral-7B-v0.1 model

### Installation

1. **Clone the repository:**
    ```bash
    [git clone https://github.com/Ammar-Abdelhady-ai/DockerCommand-Generator-LLM.git](https://github.com/Ammar-Abdelhady-ai/DockerCommand-Generator-LLM.git)
    cd DockerCommand-Generator-LLM
    ```

2. **Build and run the Docker container:**
    ```bash
    docker build -t fine-tune-mistral .
    docker run -it --gpus all fine-tune-mistral
    ```

3. **Install the required dependencies:**
    ```bash
      !pip install "unsloth[colab-new] @ git+https://github.com/unslothai/unsloth.git"
      !pip install --no-deps "xformers<0.0.27" "trl<0.9.0" peft accelerate bitsandbytes
    ```

### Usage

1. **Prepare the dataset:**
    Place your DockerNLCommands dataset in the `data/` directory.

2. **Run the fine-tuning script:**
    ```bash
    run Unsloth_mistral_7b_instruct.ipynb
    ```

3. **Generate Docker commands:**
    ```bash
    python generate_command.py --input "I want a command to build an image from a Dockerfile"
    ```

## Acknowledgments

- The developers of the Mistral-7B-v0.1 model.
- The creators of the Unsloth library for their optimized fine-tuning tools.
- The DockerNLCommands dataset contributors.

