# Azure Document Intelligence Sample

This repository contains sample code demonstrating how to use Azure Document Intelligence to extract text, layout, and other information from documents.

## Overview

Azure Document Intelligence (formerly Form Recognizer) is a cloud-based AI service that uses machine learning to extract text, key-value pairs, tables, and structure from documents. This sample demonstrates the "prebuilt-read" model which extracts text, layout information, and other elements from documents.

## Features

The sample demonstrates how to:
- Connect to Azure Document Intelligence service
- Analyze a document using the prebuilt read model
- Extract and display various elements from the document:
  - Detected languages and confidence scores
  - Text styles (handwritten content, font styles)
  - Page information (dimensions, text lines, words)
  - Selection marks (checkboxes, radio buttons)
  - Paragraphs and their content

## Prerequisites

- Python 3.7 or later
- An Azure account with an Azure Document Intelligence resource
- Azure Document Intelligence service key and endpoint

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/your-username/Azure-Doc-AI-Sample.git
cd Azure-Doc-AI-Sample
```

### 2. Set up environment

Create a virtual environment and install dependencies:

```bash
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
```

### 3. Configure credentials

Create a `.env` file in the root directory with your Azure Document Intelligence credentials:

```
DI_KEY=your_di_key
DI_ENDPOINT=your_di_endpoint
```

### 4. Run the sample notebook

Open the notebook in VS Code or Jupyter:

```bash
jupyter notebook Sample.ipynb
```

Or run with VS Code Jupyter extension.

## Project Structure

- `Sample.ipynb` - Jupyter notebook containing the sample code
- `.env` - Environment variables file (not tracked by git)
- `requirements.txt` - Python dependencies

## Security Note

This sample uses environment variables for storing credentials, which is acceptable for development. For production applications, consider using:

- Azure Key Vault for secret management
- Managed identities for Azure resources
- Azure role-based access control (RBAC) to implement least privilege access

## Dependencies

- `azure-ai-documentintelligence` - Azure Document Intelligence SDK
- `python-dotenv` - For loading environment variables from .env file

## Additional Resources

- [Azure Document Intelligence Documentation](https://docs.microsoft.com/azure/applied-ai-services/document-intelligence/)
- [Azure Document Intelligence Pricing](https://azure.microsoft.com/pricing/details/form-recognizer/)
- [Azure Document Intelligence REST API Reference](https://docs.microsoft.com/rest/api/documentintelligence/)

## Contributing

Contributions are welcome. Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
