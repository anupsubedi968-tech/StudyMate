# StudyMate — Study & Assignment Manager

StudyMate is a planned Android app for university students. It is meant to keep assignments, due dates, completion status, and exam schedules in one place on the student's phone. During a semester those notes are easy to lose, because one assignment may sit in a notebook, another in a chat message, and an exam room may be remembered only from a slide. The plan puts the unfinished work and the next exam on the same phone, stores each row locally, and shows the same lists the next time the app opens.

This folder is the **midterm planning and design** work. It is not the Android application. The app has not been built or tested.

The planning files are published at [https://github.com/anupsubedi968-tech/StudyMate](https://github.com/anupsubedi968-tech/StudyMate). GitHub can show this document. It cannot run the Android app, because that app has not been written yet. The final-term project will continue from this design.

## Student

| Item | Detail |
| --- | --- |
| Name | Subedi Anup |
| Student ID | 2025621046 |
| Course | Computer Software |
| Project | StudyMate — Study & Assignment Manager |
| GitHub account | [anupsubedi968-tech](https://github.com/anupsubedi968-tech) |
| StudyMate repository | [https://github.com/anupsubedi968-tech/StudyMate](https://github.com/anupsubedi968-tech/StudyMate) |

The repository contains this planning document and README. It does not contain an Android Studio project.

## Existing repositories on this account

Checked on 27 October 2026. These repositories are different projects and were not changed.

| Repository | What it is |
| --- | --- |
| [CampusEquipmentRentalApp](https://github.com/anupsubedi968-tech/CampusEquipmentRentalApp) | A different app. Not StudyMate. |
| [NavigationPractice](https://github.com/anupsubedi968-tech/NavigationPractice) | A Navigation practice app. Not StudyMate. |

StudyMate is a separate repository. The final-term Android project should be added there after the app is built, without deleting these planning files.

## What is in this folder

| File | Purpose |
| --- | --- |
| `StudyMate_Midterm.html` | The planning document. Open it in a browser to read it. |
| `README.md` | This explanation of the project idea, the GitHub plan, and the document. |

The professor's original brief, blank template, and sample stay in Downloads. They were not copied or changed.

## What the HTML document contains

The document follows the course template:

1. App overview, the problem, and the target user
2. Five core features, including how RecyclerView will show lists
3. Wireframes for four screens: dashboard, assignment form, assignment list, and exam schedule
4. Navigation flow between those screens
5. Two Room tables (`assignments` and `exams`) with columns, data types, and primary keys
6. How Entity, DAO, and the Room database class will save and load data on the phone
7. A week-by-week plan for building the app later, plus the GitHub plan
8. The template checklist and a short AI-use note

Section 1.4 explains that the final-term Android Studio project will continue from this design and will be added to the StudyMate repository after the app is complete and tested.

The app stays at four screens and two local tables, which matches the topics from the first eight weeks: Kotlin, Fragments, Navigation Component, RecyclerView, Room, and Git. DashboardFragment is the start screen, because a student needs a summary before an empty form. AssignmentListFragment shows the coursework, AssignmentFormFragment opens only from Add or Edit, and ExamScheduleFragment keeps the short exam form on the same screen as the exam list. The bottom bar switches only among Dashboard, Assignments, and Exams.

Room will create one SQLite file, `studymate_database`, the first time the app opens it. The `assignments` table stores the title, subject, description, due date, priority, and whether the work is pending or completed. The `exams` table stores the subject, date, time, and location. Saving a row, reading it back into a RecyclerView, marking it completed, and deleting it only after a confirmation all follow that same path. A third table is not part of this version, because the app does not store accounts or a separate subject list.
