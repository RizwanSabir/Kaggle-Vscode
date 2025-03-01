# Running VS Code on Kaggle

To set up and run VS Code on Kaggle, follow these steps:

## Prerequisites
Ensure that you have access to a Kaggle notebook with internet access enabled.

## Installation Steps
Run the following commands in a Kaggle notebook:

```bash
!pip install pyngrok
!ngrok config add-authtoken YOUR_NGROK_AUTHTOKEN
!pip install uvicorn
```

Replace `YOUR_NGROK_AUTHTOKEN` with your actual Ngrok authentication token.

## Running VS Code
After running the installation commands, execute the following command to start VS Code:

```python
ColabCode(port=1000,token="YOUR-NGROK-TOKEN")
```

Then, run the `vscode.py` file to launch VS Code in your Kaggle environment.

## Notes
- Ensure that your Ngrok token is valid.
- You may need to adjust the port number if necessary.
- This setup allows you to access VS Code remotely through Ngrok.

Enjoy coding in VS Code on Kaggle!
