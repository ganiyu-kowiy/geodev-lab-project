# My GeoDev Lab Africa Project

**Project Question:**
Which communities in Oyo State are located more than 5 km from the nearest health facility?

**Participant:** Ganiyu Kowiy Oluwasegun
**Pod:** Pod 13
**Programme:** GeoDev Lab Africa, Cohort One

Currently working on this project as part of **GeoDev Lab Africa, Cohort One**.

See **`project-brief.md`** for the full project brief.

## Month 1: GIS Foundations and Data Ecosystem

### Weekly Progress

- **Week 1 — Project Introduction and Scope:** [Project Brief](https://github.com/ganiyu-kowiy/geodev-lab-project/blob/main/project-brief.md)
- **Week 2 — Data Acquisition and Preparation:** [Data Notes](https://github.com/ganiyu-kowiy/geodev-lab-project/blob/main/data-notes.md)
- **Week 3 — Prepared Data and Quality Checks:** [Data Quality Notes](https://github.com/ganiyu-kowiy/geodev-lab-project/blob/main/data-notes.md)
- **Week 4 — Spatial Analysis and Findings:** [Month 1 Summary](https://github.com/ganiyu-kowiy/geodev-lab-project/blob/main/month-1-summary.md) | [5 km Health Facility Buffer Map](https://github.com/ganiyu-kowiy/geodev-lab-project/blob/main/5km_Buffer_Map.png)

### Month 1 Deliverables

- [Project Brief](https://github.com/ganiyu-kowiy/geodev-lab-project/blob/main/project-brief.md)
- [Data Preparation and Quality Notes](https://github.com/ganiyu-kowiy/geodev-lab-project/blob/main/data-notes.md)
- [Month 1 Summary and Findings](https://github.com/ganiyu-kowiy/geodev-lab-project/blob/main/month-1-summary.md)
- [5 km Health Facility Buffer Map](https://github.com/ganiyu-kowiy/geodev-lab-project/blob/main/5km_Buffer_Map.png)

Month 1 focused on building foundational GIS knowledge, understanding geospatial data and its sources, preparing datasets for analysis, and applying basic spatial analysis techniques.

The main project investigated **which areas in Oyo State fall outside a 5 km buffer zone around mapped health facilities**. Using QGIS, I applied the **Buffer, Dissolve, and Difference** operations to identify areas beyond the combined buffer zones.

The analysis indicated that approximately **10,265.3 km² (37.19%)** of Oyo State falls outside the 5 km buffer zones, while **62.81%** falls within them. These findings provide an initial picture of geographic proximity to mapped health facilities, although they do not directly measure road travel time, facility capacity, or the population affected.

Key learning areas included **coordinate reference systems (CRS), geospatial data acquisition, data preparation, data quality assessment, spatial operations, and geospatial data management**.

See **[Month 1 Summary and Findings](https://github.com/ganiyu-kowiy/geodev-lab-project/blob/main/month-1-summary.md)** for more details.

## Month 2: development environment and early Python
- Week 5: set up Python, VS code and terminal. hello.py runs.
- Week 6: set up the project with uv and added pandas. check.py prints the pandas version
- Week 7: analyse.py reads wards.csv, converts each area and classifies each ward.
- Week 8: inspect_data.py summarises latitude and longitude in my Oyo State health facilities data.
- Week 9: Refactored the inspection program into small functions, calculated count, smallest and largest values, handled empty data, and summarised real columns from Month 1 data.

## Month 2 Reflection — Development Environment and Early Python

Month 2 was focused on developing my foundational knowledge of Python programming and exploring how Python can be applied to data processing and analysis.

In Week 5, I installed Python, configured Visual Studio Code (VS Code) and the terminal, and successfully wrote and executed my first Python program, `hello.py`. This introduced me to the basic programming environment and how to execute Python scripts.

In Week 6, I installed and configured `uv`, verified that it was working correctly, and used it to install the `pandas` library for data manipulation and analysis.

During Week 7, I developed a Python script named `analyse.py` to read data from `wards.csv`, convert ward areas into the required units, and classify the wards based on their area values.

In Week 8, I extended my understanding of data inspection by writing code to calculate basic statistical information, including the total number of records, minimum values, and maximum values.

By Week 9, I improved my earlier inspection program by restructuring it into smaller and reusable functions. I learned how to define and call functions, return values, handle empty datasets, and summarise actual columns from my Month 1 project data.

These activities strengthened my understanding of Python fundamentals, CSV data processing, functions, and code organisation. One important lesson I learned was the value of writing reusable and well-structured code, handling possible errors or empty datasets, and separating data calculations from the presentation of results.

Overall, Month 2 marked an important step in my learning journey. I moved beyond simply setting up a programming environment and began developing practical scripts for data analysis. I now have a better understanding of how Python can support GIS workflows, automate repetitive tasks, and improve geospatial data management.

In the coming month, I look forward to improving my Python and pandas skills and exploring how programming can be integrated with GIS operations to solve practical geospatial problems.
