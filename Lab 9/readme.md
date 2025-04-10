# Setting Up a Python Virtual Environment  

Follow these steps to create and activate a virtual environment, and install dependencies from `requirements.txt`.  

## Steps  

1. **Create a Virtual Environment**  
    ```bash  
    python -m venv venv  
    ```  

2. **Activate the Virtual Environment**  
    - On **Windows**:  
      ```bash  
      .\venv\Scripts\activate  
      ```  
    - On **macOS/Linux**:  
      ```bash  
      source venv/bin/activate  
      ```  

3. **Install Dependencies**  
    ```bash  
    pip install -r requirements.txt  
    ```  

4. **Verify Installation**  
    ```bash  
    pip list  
    ```  

5. **Deactivate the Virtual Environment** (when done):  
    ```bash  
    deactivate  
    ```  

## Notes  
- Ensure you have Python installed on your system.  
- Use `python3` instead of `python` if required by your system.  
## Troubleshooting: Script Running Disabled  

If you encounter an error indicating that script execution is disabled on your system, follow these steps to enable it:  

1. Open **PowerShell** as an administrator.  
2. Run the following command to allow script execution:  
    ```bash  
    Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned  
    ```  
3. Confirm the change by typing `Y` when prompted.  

After completing these steps, try activating the virtual environment again.  