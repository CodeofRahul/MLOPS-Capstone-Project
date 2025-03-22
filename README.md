# MLOPS-Capstone-Project
This is an end to end mlops capstone project.






## **Problem Description**

When running Python scripts inside the MLOPS-Capstone-Project, i have encountered the following error:

```
Traceback (most recent call last):
  File "F:\MLOPS\MLOPS-Capstone-Project\src\data\data_ingestion.py", line 10, in <module>
    from src.logger import logging
ModuleNotFoundError: No module named 'src'
```

## **Solution: Manually Set the PYTHONPATH**

To fix this issue, we need to manually add the project root (`MLOPS-Capstone-Project`) to `PYTHONPATH` so that Python recognizes `src` as a module.

### **Steps to Fix**

**Step 1: Navigate to the Project Root**

Before running any Python script, ensure that you are inside the project’s root directory.

```
cd F:\MLOPS\MLOPS-Capstone-Project
```

### **Step 2: Set the PYTHONPATH Environment Variable**

For Windows Command Prompt (CMD):

```
set PYTHONPATH=F:\MLOPS\MLOPS-Capstone-Project
python src/data/data_ingestion.py
```

