# Drone Forensics Project

## Project Overview

This project is a digital forensics analysis of drone flight log evidence from the NIST CFReDS DroneDataSet. The purpose of this project was to examine drone-related data, identify useful evidence, and document a repeatable forensic workflow using common forensic tools.

This project is not an application or software program that I created. Instead, it is a forensic investigation and analysis project using an existing drone dataset. The goal was to show how drone evidence can be reviewed, interpreted, and documented using forensic tools.

The dataset used in this project came from the NIST CFReDS DroneDataSet. The dataset was created as part of a drone forensics program where drones were operated in a controlled environment and then examined for recoverable data. The project focused on drone flight log files, especially `.DAT` files located inside the `flight_logs` folder.

## Tools Used

The following tools were used for this project:

- FTK Imager
- CsvView
- GitHub
- Windows File Explorer
- Screenshots for documentation and results

## Dataset Used

Dataset source:

NIST CFReDS DroneDataSet  
Drone Forensics Program  
Steve Watson / VTO Inc.

The project focused mainly on drone flight log files. One of the main files examined was:

```text
FLY015.DAT
```

This file was opened in CsvView, which recognized it as a UAV flight log file.

## Repository Contents

This GitHub repository contains the project documentation and deliverables for the drone forensics project.

Recommended repository structure:

```text
Drone-Forensics-Project/
│
├── README.md
│
├── report/
│   └── project_report.docx or project_report.pdf
│
├── presentation/
│   └── project_presentation.pptx
│
├── screenshots/
│   ├── ftk_imager/
│   ├── csvview/
│   └── dataset/
│
├── results/
│   └── notes_or_summary_files.txt
│
└── data/
    └── README.md
```

Large `.DAT` files may not be included in the repository because they can exceed GitHub file size limits. If the original flight log files are too large to upload, they should be downloaded directly from the NIST CFReDS dataset.

## Important Note About Large Data Files

Some of the drone flight log `.DAT` files are too large to upload directly to GitHub. Because of this, the repository may not include every original raw data file.

To recreate the project fully, download the dataset directly from the NIST CFReDS DroneDataSet website and place the flight log files into a folder named:

```text
flight_logs
```

Example:

```text
Drone-Forensics-Project/
└── flight_logs/
    ├── FLY015.DAT
    ├── FLY016.DAT
    └── other DAT files
```

## Step-by-Step Recreation Guide

Follow these steps to recreate the project.

---

## Step 1: Download the Drone Dataset

1. Go to the NIST CFReDS DroneDataSet page.
2. Locate the DroneDataSet from Steve Watson / VTO Inc.
3. Download the available dataset files.
4. Extract the downloaded files to a folder on your computer.
5. Locate the folder containing the drone flight logs.

The flight logs should appear as `.DAT` files.

Example:

```text
FLY015.DAT
FLY016.DAT
FLY017.DAT
```

---

## Step 2: Organize the Project Folder

Create a main project folder on your computer.

Example:

```text
Drone_Forensics_Project
```

Inside the folder, create subfolders for organization:

```text
Drone_Forensics_Project/
│
├── flight_logs/
├── screenshots/
├── report/
├── presentation/
└── results/
```

Place the downloaded `.DAT` flight log files inside the `flight_logs` folder.

---

## Step 3: Open the Dataset in FTK Imager

FTK Imager was used to view the dataset from a forensic evidence perspective.

1. Open FTK Imager.
2. Select:

```text
File > Add Evidence Item
```

3. Choose the option that matches the evidence source.
4. For this project, the evidence was reviewed from files and folders, so the folder containing the drone dataset was added.
5. Navigate to the extracted drone dataset folder.
6. Add the folder as an evidence item.
7. Expand the folder structure inside FTK Imager.
8. Locate the `flight_logs` folder.
9. Select one or more `.DAT` files.

FTK Imager can show the raw file structure and hexadecimal data. This helps prove that the evidence files exist and allows the investigator to view the raw data, even if the file is not easily readable as normal text.

### Screenshots to Capture in FTK Imager

Capture screenshots showing:

- The dataset folder loaded as evidence
- The `flight_logs` folder
- A selected `.DAT` file
- The raw hex/data view of the selected file

These screenshots document that the original evidence was reviewed using a forensic tool.

---

## Step 4: Open a Flight Log in CsvView

CsvView was used to interpret the `.DAT` drone flight log files.

1. Open CsvView.
2. Select the option to open a log file.
3. Navigate to the `flight_logs` folder.
4. Select a `.DAT` file.

Example:

```text
FLY015.DAT
```

5. Open the file.
6. Allow CsvView to process the file.
7. Confirm that CsvView recognizes the file as a UAV flight log.

CsvView provides a more readable view of the flight data compared to FTK Imager because it can interpret drone log data and display flight-related information.

---

## Step 5: Review the Flight Log Data in CsvView

Once the `.DAT` file is opened in CsvView, review the available data sections.

Important areas to examine include:

- GPS or location-related data
- Altitude values
- Flight time or timestamp information
- Speed or movement values
- Battery or power information
- Sensor or aircraft status information
- Any graphs or data tables available in CsvView

The purpose of this step is to identify what useful forensic evidence can be recovered from the drone flight log.

---

## Step 6: Capture CsvView Screenshots

Take screenshots of important CsvView sections.

Recommended screenshots include:

- The `.DAT` file successfully opened in CsvView
- The file name visible in the program
- Any summary or overview page
- Graphs showing altitude, speed, or flight behavior
- Tables showing GPS, time, or sensor data
- Any section that shows the file was recognized as a UAV log

These screenshots serve as project evidence and support the final presentation and report.

---

## Step 7: Document Findings

Create a notes file or results file summarizing what was found.

Example results file:

```text
results/flight_log_analysis_notes.txt
```

The notes should include:

- Name of the flight log examined
- Tool used to examine the file
- Whether the file opened successfully
- Types of data observed
- Any important forensic observations

Example:

```text
FLY015.DAT was opened in CsvView and recognized as a UAV flight log.
The file contained flight-related data that could be reviewed through CsvView.
FTK Imager was also used to verify the file structure and view the raw evidence data.
```

---

## Step 8: Prepare the Project Report

The final report should explain:

- The purpose of the project
- The dataset used
- The forensic tools used
- The steps taken during the analysis
- The evidence reviewed
- The findings from FTK Imager and CsvView
- The limitations of the project
- The conclusion

The report should make clear that this project is a forensic workflow and evidence analysis project, not a custom-built application.

---

## Step 9: Prepare the Project Presentation

The presentation should explain the project in a clear sequence:

1. Introduction
2. Dataset background
3. Tools used
4. FTK Imager workflow
5. CsvView workflow
6. Findings
7. Limitations
8. Conclusion

The presentation should include screenshots from FTK Imager and CsvView to show that the project was completed and that the evidence was examined.

---

## Step 10: Upload Project Files to GitHub

Upload the final project materials to GitHub.

Recommended files and folders to upload:

```text
README.md
report/
presentation/
screenshots/
results/
```

If the `.DAT` flight logs are too large for GitHub, do not upload them directly. Instead, explain in the README that the raw dataset must be downloaded from NIST CFReDS.

---

## Step 11: Verify the GitHub Repository

Before submission, check that the repository includes:

- Final presentation slides
- Project report
- Screenshots
- Results or notes
- README.md recreation guide
- Explanation of where the original dataset came from
- Explanation of how to recreate the analysis

The README.md file should allow another person to follow the same steps and recreate the project using the same dataset and tools.

## Forensic Summary

This project demonstrates a basic drone forensics workflow. FTK Imager was used to view and verify the evidence files from a forensic perspective, while CsvView was used to interpret the drone `.DAT` flight logs in a readable format. The project shows that UAV flight logs can contain important evidence such as flight activity, movement data, and sensor-related information.

The main forensic value of the project is showing how raw drone files from a dataset can be examined, documented, and explained as part of a digital forensic investigation.

## Limitations

This project has several limitations:

- Some `.DAT` files may be too large to upload to GitHub.
- FTK Imager can show the raw file data, but it does not fully interpret drone flight logs.
- CsvView is needed to make the UAV log data easier to understand.
- The project depends on the available NIST dataset files.
- The analysis focuses on available flight log evidence rather than a full physical drone investigation.

## Conclusion

The project successfully demonstrates how drone forensic evidence can be examined using FTK Imager and CsvView. The NIST CFReDS DroneDataSet provided realistic drone evidence files, and the analysis focused on identifying and documenting flight log data. Through this workflow, the project shows how digital forensic tools can be used to recover and interpret drone-related evidence.

## References

NIST CFReDS DroneDataSet  
https://cfreds.nist.gov/all/SteveWatson%2FVTOInc./DroneDataSet

FTK Imager  
https://www.exterro.com/ftk-imager

CsvView  
https://datfile.net/CsvView/intro.html
