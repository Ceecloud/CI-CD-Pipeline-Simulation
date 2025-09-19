# CI/CD Pipeline Simulation

![Deploy an EC2](https://github.com/Ceecloud/CI-CD-Pipeline-Simulation/actions/workflows/pipeline.yaml/badge.svg)
CI/CD Pipeline Simulation

This repository demonstrates a simple CI/CD pipeline using GitHub Actions.
The pipeline simulates deploying an EC2 instance and runs multiple jobs sequentially.

Project Structure
CI-CD-Pipeline-Simulation/
│── index.html # Basic HTML file
│── app.js # Simple JavaScript file
│── README.md # Project documentation
└── .github/
└── workflows/
└── pipeline.yaml # GitHub Actions workflow

Workflow Overview

The pipeline consists of four sequential jobs:

Deploy1 – Checks out the repo and lists files.

Deploy2 – Reads the index.html file.

Deploy3 – Lists files again.

Deploy4 – Reads the index.html file again.

Jobs are chained using the needs: keyword so they run one after the other.

How to Use

Clone this repository:

git clone https://github.com/Ceecloud/CI-CD-Pipeline-Simulation.git
cd CI-CD-Pipeline-Simulation

Push changes to the cicd branch:

git checkout cicd
git add .
git commit -m "update"
git push origin cicd

Check the Actions tab in GitHub to see the workflow run.

Example Output

✅ ls -la shows all files in the repo

✅ cat index.html displays the HTML content

Purpose

This project is only for learning and simulation.
It does not deploy a real EC2 instance but demonstrates the workflow of a CI/CD pipeline.

Once you save it, just run:

git add README.md
git commit -m "Final clean README"
git push origin cicd
