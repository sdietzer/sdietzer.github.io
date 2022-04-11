---
title: "python venv commands"
date: 2022-04-08T23:24:28-04:00
draft: false
---
 
create a virtual environment in current directory
```python
python -m venv my_venv
```

create a virtual environment in a specific dirctory
```python
python3 -m venv path/to/your/venv/my_venv
```

activate a virtual environment using powershell from the venv/scripts folder
```powershell
./Activate.ps1
```

deactivate a virtual environment using powershell from the venv/scripts folder
```powershell
deactivate
```

remove/delete a virtual environment (just delete the directory)
```powershell
rm -rf /path/to/my_venv
```

clear an existing virtual environment
```python
python -m venv --clear path/to/my_venv
```










:earth_africa: