# **STUDENT MARKS ANALYZER** ( Version 2 )

A command-line tool written in Python that turns a student's subject marks into a clear performance report: pass/fail status per subject, overall percentage, grade, and a bar chart to go with it.

This is the **second version** of the project. The first version worked with a fixed set of subjects. This one lets you choose how many subjects to enter and checks every input along the way.

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Charts-orange)
![Version](https://img.shields.io/badge/Version-2.0-green)

---

## What's new in Version 2

- Choose any number of subjects instead of a fixed list
- Friendly prompts that count along: "1st subject", "2nd subject", "3rd subject"
- Input validation for subject count, names and marks
- Duplicate subject names are rejected
- Results table with Name, Score and Status columns
- Highest and lowest scoring subjects
- Bar chart built with Matplotlib, with a pass-mark line

## Features

- Marks must be between 0 and 100
- Subject names are cleaned up automatically (`mths` becomes `Mths`)
- Pass mark is 45 per subject (easy to change)
- Overall percentage and grade
- Chart colours: green for pass, red for fail

## Libraries used

| Library | Purpose |
|---|---|
| `matplotlib` | Draws the bar chart of subject marks |

Everything else (`input`, `print`, string formatting) is plain Python, so Matplotlib is the only thing you need to install.

## Getting started

```bash
git clone https://github.com/Rammal-Ahmed/student-performance-report-v2.git
cd student-performance-report-v2
pip install -r requirements.txt
python main.py
```

The script also runs fine inside Jupyter Notebook.

## Grading scale

| Percentage | Grade |
|---|---|
| 90 and above | A |
| 80 to 89 | B |
| 70 to 79 | C |
| 60 to 69 | D |
| 46 to 59 | E |
| Below 45 | Fail |

A subject is marked **Pass** when the score is 45 or higher.

## Sample run

```
========================================
     STUDENT MARKS ANALYSIS REPORT
========================================

Specify the total number of subjects: 3
----------------------------------------

Enter name of 1st subject: maths

Enter marks of 1st subject (Maths) (0-100): 82


Enter name of 2nd subject: physics

Enter marks of 2nd subject (Physics) (0-100): 74


Enter name of 3rd subject: english

Enter marks of 3rd subject (English) (0-100): 41


..............................
     Subject-wise Status
..............................
Name             Score   Status
------------------------------
Maths             82.0   Pass
Physics           74.0   Pass
English           41.0   Fail

...............
    Result
...............
Total: 197.0
Highest: 82.0 (Maths)
Lowest: 41.0 (English)
Percentage: 65.67%
Grade: D
```

After the report, a bar chart opens showing every subject against the pass mark.

## Project structure

```
student-performance-report-v2/
├── main.py
├── requirements.txt
├── README.md
└── .gitignore
```

## Ideas for the next version

- Save the report to a text or CSV file
- Support multiple students in one run
- Add weighted subjects

## About me

# **Rammal Ahmed**

**AI & Data Science Enthusiast** | **Microsoft Dynamics 365 CRM Developer** | **Power Platform** | **UI/UX Designer** | **Graphic Designer & Illustrator**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/rammal-ahmed-58184b325)
[![GitHub](https://img.shields.io/badge/GitHub-Rammal--Ahmed-181717?style=flat&logo=github)](https://github.com/Rammal-Ahmed)

<div align="center">

If you found this useful, consider giving it a star ⭐

**I truly value your feedback and welcome any suggestions for improvement**

**Always open to fresh perspectives, constructive feedback, and new ideas**


## License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details

---

*Developed as part of my Python programming practice*

---

**Project Status:** Completed

</div>
