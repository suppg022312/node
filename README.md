# Node.js & Python Development Environment with Docker

This repository contains a development environment setup using Docker Compose, providing a containerized environment with Node.js, Python, and Jupyter Notebook.

## Setup

1.  **Prerequisites:**
    *   Docker and Docker Compose installed on your system.

2.  **Clone the repository:**
    ```bash
    git clone https://github.com/suppg022312/node.git
    cd node
    ```

3.  **Build and run the container:**
    ```bash
    docker-compose up -d --build
    ```

## Accessing Jupyter Notebook

Once the container is running, you can access Jupyter Notebook by opening the following URL in your web browser:

[http://localhost:8888](http://localhost:8888)

**Note:**  Token authentication for Jupyter Notebook is currently disabled for local development convenience.  Do *not* use this configuration in a production environment without enabling authentication.

## Included Libraries
- Python
- Node.js
- SQLAlchemy
- Gradio
- Streamlit
- uv
- Jupyter

## MCP Servers
This project is set up to be used in conjunction with Model Context Protocol (MCP) servers. You can find available MCP servers in the [MCP Marketplace](https://github.com/cline/mcp-marketplace).

Further configuration is required to set up specific MCP servers, such as those for accessing Microsoft services (Outlook, SharePoint) via the Microsoft Graph API. This typically involves creating an app registration in Azure Active Directory and configuring the server with the appropriate credentials.