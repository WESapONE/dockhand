# dockhand - WesLab
# ⚓ WesLab's Dockhand

[![GitHub last commit](img.shields.io)](img.shields.io)
[![License: MIT](img.shields.io)](opensource.org)

A collection of Docker Compose files, configuration scripts, and documentation for managing services in my personal homelab environment. This repository serves as the central "dockhand" for orchestrating all the self-hosted services.

---

## 🌟 Highlights

*   **Infrastructure as Code:** Manage services using version-controlled Docker Compose files.
*   **Automated Setup:** Simple scripts to get services up and running quickly.
*   **Centralized Documentation:** A single source of truth for configurations, IP addresses, and service access.

---

## 🚀 Getting Started

These instructions will get your local copy WesLab's services up and running.

### ⚙️ Prerequisites

Before you begin, ensure you have the following installed on your host machine:

*   **Docker:** Used for containerization.
*   **Docker Compose:** For defining and running multi-container Docker applications.
*   **Git:** For cloning the repository.

### ⬇️ Installation and Setup

1.  **Clone the repository:**
    ```bash
    git clone github.com
    cd YOUR_REPO_NAME
    ```

2.  **Configure Environment Variables (Optional but Recommended):**
    Copy the sample environment file and update the values as needed (e.g., specific ports, volume paths, passwords).
    ```bash
    cp .env.example .env
    # Edit the .env file with your preferred text editor
    ```

3.  **Deploy the Services:**
    Use Docker Compose to start all the defined services. The `-d` flag runs them in detached mode.
    ```bash
    docker-compose up -d
    ```

---

## 📋 Services Overview

Here is a list of services currently running in my homelab and their primary access points:

*   **Homarr (Dashboard):** [http://(http://172.16.15.48:7575) - *Central dashboard for accessing all services*.
*   **Portainer (Container Management):** [http://172.16.15.38:9443) - *Web UI for managing Docker containers*.
*   **technitium (Network-wide Ad Blocking):** [(http://172.16.15.43:5380/)] - *DNS-level ad blocking*.
*   **pangolin (Self-hosted Oracle-cloud proxy):** [(https://pangolin.mintdynastyresearch.org)] - *Private proxy*.
*   ... *Add more services as needed*

---

## 📂 Project Structure

The repository is organized as follows:

*   `./`: The root directory contains the main `docker-compose.yml` file and this README.
*   `./config/`: Configuration files for various services.
*   `./scripts/`: Utility scripts for backup, updates, or maintenance.
*   `./documentation/`: Detailed notes, network diagrams, and weird config notes.

---

## 🤝 Contributing

This is a personal homelab repository, but feedback, suggestions, or ideas are welcome! Feel free to open an issue or fork the repository.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE) - see the `LICENSE` file for details.

---

## acknowledgments

Inspiration for this setup came from various sources in the homelab community on GitHub and Reddit.

