# FILE-RECOVERY-USING-AUTOPSY-SOFTWARE
### NAME - TH KARTHIK KKRISHNA
### REG NO - 212223240067
## AIM
To use **Autopsy Digital Forensics Tool** to retrieve deleted files from a disk image.

---

## REQUIREMENTS
- **Operating System**: Windows 10/11, macOS, or Linux
- **Tool**: [Autopsy Digital Forensics](https://www.autopsy.com/)  
- **Test Data**: Disk image file (`disk.dd`, `disk.img`, `.E01`)

---

## ARCHITECTURE DIAGRAM
```mermaid
flowchart TD
    A[Disk Image / Physical Drive] --> B[Install Autopsy]
    B --> C[Create New Case in Autopsy]
    C --> D[Add Data Source: Disk Image]
    D --> E["Run File System & Data Recovery Modules"]
    E --> F[Locate Deleted Files in Results]
    F --> G[Recover and Export Deleted Files]
```
## DESIGN STEPS:
### Step 1:
Open Autopsy and create a new case with appropriate case details.

### Step 2:
Add a disk image as a data source and let Autopsy analyze the content.

### Step 3:
Navigate to the "Deleted Files" section in Autopsy and examine or recover the deleted files.

## PROGRAM:
### Install Autopsy
```bash
# Download Autopsy from:
# https://www.autopsy.com/
# Install following the setup wizard.
```
### Create a New Case
```
# File → New Case
# Enter Case Name: Deleted_File_Recovery
# Choose Base Directory: C:\Cases\Deleted_File_Recovery
# Click Finish
```
### Add Disk Image
```
# Add Data Source → Disk Image or VM File
# Browse to: C:\forensics\disk.dd
# Click Next
```
### Run Ingest Modules
```# Select:
# - File System Analysis
# - Keyword Search (optional)
# - Data Recovery / Carving
# Click Finish
```
### Locate Deleted Files
```
# Navigate to 'Deleted Files' section in the tree view
# Review metadata (size, hash, timestamps)
```
### Export Deleted Files
```
# Right-click → Extract File(s)
# Save to: C:\forensics\Recovered_Files\
```

## OUTPUT:
Recovered Deleted File List and Details
<img width="1600" height="899" alt="image" src="https://github.com/user-attachments/assets/5f0a9ade-b10b-4723-aead-36763df532bb" />
<img width="1600" height="899" alt="image" src="https://github.com/user-attachments/assets/9889823b-2a01-4d19-8154-d14b5a180a41" />
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/6d72bccf-f947-451b-aa20-c13ab2b5b838" />
<img width="1600" height="899" alt="image" src="https://github.com/user-attachments/assets/4e957c87-8c26-4ea1-86aa-44cba53a1313" />
<img width="1600" height="892" alt="image" src="https://github.com/user-attachments/assets/223740e4-7d3f-4f78-b00e-acc9bb8ed383" />
<img width="1600" height="899" alt="image" src="https://github.com/user-attachments/assets/ffd0aa4b-d05f-49d1-aaf2-f2ee38f8276e" />
<img width="1600" height="898" alt="image" src="https://github.com/user-attachments/assets/b5bf423f-1a59-47f1-bc27-0bc3653de3fa" />
<img width="1600" height="899" alt="image" src="https://github.com/user-attachments/assets/a541edac-697a-4972-a3e0-72cd4464e8dd" />
<img width="1600" height="895" alt="image" src="https://github.com/user-attachments/assets/e0b06834-8382-40e1-b1e8-c4581253f3e2" />
<img width="1600" height="899" alt="image" src="https://github.com/user-attachments/assets/7a4d95ae-0825-42e1-8102-092ffd0f1606" />
<img width="1482" height="926" alt="image" src="https://github.com/user-attachments/assets/0229fd38-0baf-43f6-92d1-123e78202f53" />


## RESULT:
Deleted files were successfully retrieved and analyzed using Autopsy.
