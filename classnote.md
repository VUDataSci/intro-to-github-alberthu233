### File names
- Machine-readable
    - avoid spaces, punctuation, characters
- Human-readable
    - info and readable URL slug format
- Defalt-ordering
    - left pad numbers
    - date format YY-MM-DD


```python
# quick example provided by copilot
import os

# Machine-readable file name
machine_readable_name = "example_file.txt"
machine_readable_name = machine_readable_name.replace(" ", "_").lower()
print(f"Machine-readable file name: {machine_readable_name}")

# Human-readable file name
human_readable_name = "Example File Name"
human_readable_name = "-".join(human_readable_name.lower().split())
print(f"Human-readable file name: {human_readable_name}")

# Default-ordering file name
file_number = 1
file_date = "2022-01-01"
default_ordering_name = f"{str(file_number).zfill(3)}_{file_date}_{machine_readable_name}"
print(f"Default-ordering file name: {default_ordering_name}")

# Create file with default-ordering name
with open(default_ordering_name, "w") as f:
    f.write("Example file content")
```

    Machine-readable file name: example_file.txt
    Human-readable file name: example-file-name
    Default-ordering file name: 001_2022-01-01_example_file.txt


### Software Set-up
- git and github
- anaconda
- python
- jupyter
