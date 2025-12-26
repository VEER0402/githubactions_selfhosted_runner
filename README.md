# GitHub Actions CI/CD with Self-Hosted Runner

## Overview

This project demonstrates a **production-style CI/CD pipeline** implemented using **GitHub Actions with a self-hosted Linux runner**.
Instead of relying on GitHub-hosted runners, the pipeline is executed on a **dedicated Linux machine**, providing better control, flexibility, and real-world CI/CD exposure.

The setup closely mirrors how organizations run CI/CD pipelines on their **own infrastructure** for security, cost optimization, and performance reasons.

---

## Problem Statement

GitHub-hosted runners are convenient but have limitations:

* Limited control over the execution environment
* Cold start delays
* Restricted access to internal infrastructure
* Not suitable for long-running or infra-heavy workloads
* Cost implications at scale

In real-world DevOps environments, teams often need:

* Full OS-level control
* Ability to install custom tools & dependencies
* CI/CD execution inside private networks
* Predictable and reusable runners

---

## Solution

This project solves the above challenges by:

* Configuring a **self-hosted GitHub Actions runner** on a Linux machine
* Executing CI/CD workflows on custom infrastructure
* Integrating the runner seamlessly with GitHub Actions workflows

The pipeline is triggered automatically on repository events and runs jobs on the self-hosted runner using the `self-hosted` label.

---

## Key Features

* ✅ Self-hosted GitHub Actions runner on Linux
* ✅ Custom CI workflow using YAML
* ✅ Full control over runner environment
* ✅ Faster and predictable job execution
* ✅ No dependency on GitHub-hosted runners
* ✅ Suitable for enterprise and on-prem setups

---

## CI/CD Workflow Highlights

* GitHub Actions workflow defined under `.github/workflows/`
* Jobs explicitly configured to run on:

  ```
  runs-on: self-hosted
  ```
* Runner registered and managed from repository settings
* Secure communication between GitHub and runner via authentication token

---

## Use Cases

This setup is ideal for:

* Enterprise CI/CD pipelines
* On-prem or private cloud environments
* Infrastructure-heavy builds
* Docker, Kubernetes, or Terraform pipelines
* Cost-optimized CI/CD at scale
* Compliance-driven environments

---

## Impact & Value

* 🔹 Reduced CI/CD execution cost
* 🔹 Improved control over build environment
* 🔹 Production-ready CI/CD architecture
* 🔹 Real-world DevOps implementation (not demo-level)
* 🔹 Resume-ready project demonstrating hands-on CI/CD expertise

---

## Tech Stack

* GitHub Actions
* Self-hosted Runner (Linux)
* YAML-based CI configuration
* Git & GitHub

---

## Project Ownership

This project is implemented and customized as part of hands-on DevOps practice to simulate **real production CI/CD workflows** using self-hosted infrastructure.

---

![github](https://github.com/user-attachments/assets/c368695d-cbe3-4e6c-86fe-0e7e91dc37dc)

---

⭐ **This project reflects real-world CI/CD practices using GitHub Actions and self-hosted runners.**

