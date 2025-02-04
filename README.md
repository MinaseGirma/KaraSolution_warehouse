# KaraSolution_warehouse


## Project Overview

This project involves building a complete data pipwarehouseeline to scrape, clean, and store data on Ethiopian medical businesses. The final product includes an integrated data warehouse and a FastAPI backend to expose the data. Object detection using YOLO is implemented to enhance the data analysis by processing images collected from various Telegram channels.

### Key Features:

1. **Telegram Data Scraping**: Scrape relevant business data from public Telegram channels using `telethon` and Python scripts.
2. **ETL/ELT Data Transformation**: Clean and transform the data using **DBT (Data Build Tool)** for structured data in the warehouse.



## Project Structure

```plaintext

Ethio-Medical-Data-Warehouse/
├── .vscode/
│   └── settings.json
├── .github/
│   └── workflows/
│       └── unittests.yml               # GitHub Actions
├── src/
│   └── __init__.py
├── notebooks/
|   ├── to_postgres.ipynb                        # Jupyter notebook for exporting to postgres
|   ├── yollo.ipynb                              # Jupyter notebook for object detection
│   └── README.md                                # Description of notebooks directory 
├── tests/
│   └── __init__.py
├── scripts/
|    ├── __init__.py
│    ├── tl_scrapper.py                          # Script data processing, cleaning 
│    └── README.md                               # Description of scripts directory
│
├── requirements.txt                             # Python dependencies
├── README.md                                    # Project documentation
├── LICENSE                                      # License information
└── .gitignore                                   # Files and directories to ignore in Git  
```

## Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/MinaseGirma/KaraSolution_warehouse.git
   cd KaraSolution_warehouse


2. Create a virtual environment:
   ```bash
   python -m venv venv
   venv\Scripts\activate  # On Linux, use `source venv/bin/activate`
   

3. Install the required packages:
   ```bash
   pip install -r requirements.txt