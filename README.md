# Healthcare Data Engineering Project


# Azure Storage Structure

The Azure Data Lake Storage Gen2 container used in this project is organized as follows:


Container: healthecare
│
├── JSON landingFile
│   ├── 557 FHIR JSON files
│
├── landing
│   ├── FHIRfiledata
│   │   └── FHIR JSON files copied by Azure Data Factory
│   │
│   ├── HospitalCostFileData
│   │   └── Hospital Cost Report CSV
│   │
│   ├── ICDfileData
│   │   └── ICD Code File
│   │
│   └── MUPfiledata
│       └── Medicare Prescriber Data (Loaded through SHIR)
│
└── ProcessData
    ├── Bronze
    ├── Silver
    └── Gold


## Folder Description

| Folder | Description |
|---------|-------------|
| JSON landingFile | Contains 557 raw FHIR JSON files uploaded from local machine. |
| landing/FHIRfiledata | Raw FHIR files copied by Azure Data Factory pipeline. |
| landing/HospitalCostFileData | Hospital Cost Report CSV file. |
| landing/ICDfileData | ICD code reference file. |
| landing/MUPfiledata | SHIR copies on-premise Medicare Prescriber data into this folder. |
| ProcessData/Bronze | Raw data processed by Databricks. |
| ProcessData/Silver | Cleaned and transformed data. |
| ProcessData/Gold | Business-ready curated data for reporting and analytics. |
