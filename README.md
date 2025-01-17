# 📍 ZIP Code Lookup - FastAPI Project  
This project was developed to offer a complete service for querying, managing, and exporting ZIP codes, using Python, FastAPI, and MongoDB.

## 🎯 Goal  
Develop a system that:  

- **ZIP Code Lookup**: Allows searching for ZIP codes using the ViaCEP API.  
- **Storage**: Saves query results in a MongoDB database.  
- **Export**: Provides the option to export data in JSON or CSV formats.  
- **CRUD Operations**: Implements CRUD operations (Create, Read, Update, and Delete) to manage stored data.  

## ✨ Features  

1. **ZIP Code Lookup** 🔍  
   - Search ZIP codes by state and specific ZIP code.  
   - Utilizes the ViaCEP API to fetch data.  
   - Includes validation to ensure integrity and handle errors effectively.  

2. **Storage in MongoDB** 🗂️  
   - Saves query data in MongoDB.  
   - Prevents duplication by verifying records before saving.  

3. **Data Export** 📤  
   - Stored data can be exported as:  
     - **JSON**: Structured for integration or API usage.  
     - **CSV**: For data analysis or spreadsheet manipulation.  

4. **CRUD Operations** 🔧  
   - **Create**: Manually add a ZIP code record.  
   - **Read**: List all stored ZIP codes.  
   - **Update**: Update data for a specific ZIP code.  
   - **Delete**: Remove unwanted records.  

## 🛠️ Technologies Used  

- **Python** 🐍: Main programming language.  
- **FastAPI** ⚡: Framework for API development.  
- **MongoDB** 🍃: NoSQL database for storage.  
- **ViaCEP API** 📡: Service for ZIP code lookup.  
- **Postman** 📬: Tool for endpoint testing and validation.  

### 📚 Additional Libraries  

- **pymongo**: MongoDB connection.  
- **csv, json**: Data manipulation and export.  
- **requests**: External API consumption.  

## 🚀 Installation  

Clone the repository:  

```bash  
git clone https://github.com/your-username/zip-code-lookup.git  
cd zip-code-lookup  
```  

Install dependencies:  

```bash  
pip install -r requirements.txt  
```  

Configure MongoDB:  

Ensure MongoDB is installed and running on the default port.  

Start the service:  

```bash  
python zip_code_lookup.py  
```  

## 🔧 Usage  

### API Endpoints  

- **POST /create/**: Creates a new ZIP code record.  
- **GET /read/**: Lists all stored ZIP code records.  
- **PUT /update/{zip_code}/**: Updates data for a specific ZIP code.  
- **DELETE /delete/{zip_code}/**: Deletes a ZIP code record.  

### Available Scripts  

- **Export to JSON**:  
  ```bash  
  python zip_code_lookup.py --export json  
  ```  

- **Export to CSV**:  
  ```bash  
  python zip_code_lookup.py --export csv  
  ```  

## 📁 Repository Files  

- `zip_code_lookup.py`: Main script implementing the service.  
- `queries.json`: Example export in JSON format.  
- `queries.csv`: Example export in CSV format.  
