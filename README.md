# Project2-TDS

## **How to Run the App Locally**

To run the app on your local machine, follow these steps:

### **1. Clone the Repository**
First, clone the repository to your local machine:
```bash
git clone https://github.com/your-username/TDS-project-2.git
cd TDS-project-2
```

### **2. Set Up a Virtual Environment**
Create and activate a virtual environment to manage dependencies:
```bash
python3 -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
```
or use uv 

```bash
uv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
```

### **3. Install Dependencies**
Install the required Python packages:
```bash
pip install -r requirements.txt
```

or use uv
```bash
uv pip install -r requirements.txt
```

### **4. Set Up Environment Variables**
Create a `.env` file in the project root and add the necessary environment variables:
```env
AIPROXY_TOKEN=your_openai_api_key
```

### **5. Run the Application**
Start the Flask development server:
```bash
python -m api.app
```

The app will be available at `http://127.0.0.1:8000`.

### **6. Test the API**
You can test the API using tools like `curl` or Postman. For example:
```bash
curl -X POST "http://127.0.0.1:8000" \
  -H "Content-Type: multipart/form-data" \
  -F "question=What is the output of code -s in VS Code?"
```

### **7. Stop the Server**
To stop the server, press `Ctrl+C` in the terminal.