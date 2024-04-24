# Backend Documentation

## Introduction

This document describes the backend services for our project, which is built using [Quart](https://quart.palletsprojects.com/), a Python framework for asynchronous web applications.

## Getting Started

### Prerequisites

- Python 3.11
- Quart

### Installation

To set up the backend, follow the steps in the `app/start.sh` or `app/start.ps1` scripts. These scripts create a Python virtual environment, install the necessary Python packages, and start the backend server.

## Backend Structure

The backend code is stored in the `app/backend` folder. The frontend and backend communicate using the [AI Chat App HTTP Protocol](https://github.com/Azure-Samples/ai-chat-app-protocol).

The `app/backend/approaches` folder contains the classes powering the Chat and Ask tabs. Each class uses a different RAG (Retrieval Augmented Generation) approach.

## Customizing the Backend

You can customize the backend by modifying the code in the `app/backend/approaches` folder. For example, the `app/backend/approaches/chatreadretrieveread.py` file contains the approach used for the Chat tab.

## Deployment

The backend is deployed using Azure's App Service, as defined in the `infra/main.bicep` file. The backend uses a managed identity and communicates with various Azure services, such as Azure AI Search and Azure Storage.

## Testing

Testing instructions will be added here.

## Contributing

Instructions on how to contribute to the backend code will be added here.

## Authors

- John Doe
- Jane Smith
- Alex Johnson

## License

This project is licensed under the MIT License. See the [LICENSE](/c:/Users/azureuser/source/repos/azure-search-openai-demo/app/backend/LICENSE) file for more information.

## Acknowledgments

Any acknowledgments if necessary will be added here.