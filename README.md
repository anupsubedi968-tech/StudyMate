# StudyMate — Study & Assignment Manager

StudyMate is a planned Android app that helps one university student keep assignments, due dates, completion status, and exam details together on their own phone. During a semester those notes are easy to lose, because one assignment may sit in a notebook, another in a chat message, and an exam room may be remembered only from a slide. This plan puts the unfinished work and the next exam in one place, stores each row locally, and shows the same lists the next time the app opens.

This repository is the midterm planning and design work. The Android application has not been built or tested, so GitHub can show the plan and cannot run an app yet. The final-term project will continue from this design.

## Student

| Item | Detail |
| --- | --- |
| Name | Subedi Anup |
| Student ID | 2025621046 |
| Course | Computer Software |
| Project | StudyMate — Study & Assignment Manager |
| GitHub account | [anupsubedi968-tech](https://github.com/anupsubedi968-tech) |
| StudyMate repository | [https://github.com/anupsubedi968-tech/StudyMate](https://github.com/anupsubedi968-tech/StudyMate) |
| Document date | 2026-10-27 |

The repository holds the planning document and this README. It does not hold an Android Studio project.

## Other repositories on this account

On 27 October 2026 the account already contained two different projects. They were left unchanged, and StudyMate was created as its own repository so those projects stay as they are.

| Repository | What it is |
| --- | --- |
| [CampusEquipmentRentalApp](https://github.com/anupsubedi968-tech/CampusEquipmentRentalApp) | A different app. Not StudyMate. |
| [NavigationPractice](https://github.com/anupsubedi968-tech/NavigationPractice) | A Navigation practice app. Not StudyMate. |

## What is in this repository

| File | Purpose |
| --- | --- |
| `StudyMate_Midterm.html` | The 8-page planning document. Open it in a browser, then print or save it as PDF. |
| `README.md` | This explanation of the idea, the GitHub plan, and how to export the PDF. |
| `.gitignore` | Ignores `.DS_Store` only. An Android `.gitignore` will be added when the app exists. |

The professor's original brief, blank template, and sample stay in Downloads. They were not copied or changed.

## What the plan covers

The document follows the course template and stays inside the topics from the first eight weeks: Kotlin, Fragments, Navigation Component, RecyclerView, Room, and Git.

The app is planned as four screens and two local tables. DashboardFragment is the start screen, because a student needs a summary before an empty form. AssignmentListFragment shows the coursework, AssignmentFormFragment opens only from Add or Edit, and ExamScheduleFragment keeps the short exam form on the same screen as the exam list so the app does not need a fifth fragment. The bottom bar switches only among Dashboard, Assignments, and Exams.

Room will create one SQLite file, `studymate_database`, the first time the app opens it. The `assignments` table stores the title, subject, description, due date, priority, and whether the work is pending or completed. The `exams` table stores the subject, date, time, and location. Saving a row, reading it back into a RecyclerView, marking it completed, and deleting it only after a confirmation all follow that same write-then-read path. A third table is not part of this version, because the app does not store accounts or a separate subject list.

## How to make the PDF

Open `StudyMate_Midterm.html` in Chrome, use Print, set the paper to A4, set the margins to None, and turn on background graphics. Save the file as `Midterm_2025621046_SubediAnup.pdf`. The document date inside the HTML is 2026-10-27, so change that date if you submit on a different day. The assignment brief lists the deadline as 31 October 2026, 23:59, and it labels that date as a proposed schedule, so confirm the real deadline with the professor or the course page. Submit the PDF. This README is the explanation that stays with the repository.

## Later, when the app is ready

After the Android Studio project is built and tested, it will be added to this same repository beside the planning files. The README will then explain how to open and run the app, an Android `.gitignore` will keep build folders out of the upload, and the project will be checked so that no passwords or keys are included. The planning files stay, and `CampusEquipmentRentalApp` and `NavigationPractice` stay unchanged.

Cursor (Grok) drafted this plan from the StudyMate idea and the course template, then uploaded these planning files. The Android app was not built or tested.
