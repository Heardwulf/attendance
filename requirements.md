# Requirement notes

Written by [John Earl Hardesty](mailto:john-hardesty@uiowa.edu) on 2020-02-25

1 min 24 sec reading time



## Problem

Registrar Office requires attendance taken for various financial aid situations. However, that can be a time-consuming process in class sizes of hundreds of students. 



## Expectation

The solution is an attendance app. The term *app* was not defined. Given the scope of the project and course level, we can infer the solution would be web-based and leverage languages we understand. 



## Requirements

This app should:

- Be automated
- Scalable to allow hundreds of students to record attendance 
- Record responses only when students are in the room or close enough
- Gracefully handle situations when students have no device

### Use case for an instructor

- Put up a slide during a lecture with directions
- Students follow directions on their smartphone or laptop
*  *This implies a temporal component as a suggestion*
- If a student is unable to use the app, they should be able to sign a sheet of paper from the instructor

### Current solutions

* Quizzes through ICON
  * Temporal restrictions may lead to students missing the quiz window
  * Quizzes for the sole purpose of attendance tracking
* Clicker apps
  *Require students to pay for a subscription

### Suggested approaches

* Location (GPS) or network (Wi-Fi access point specific) possible
  * How would students not on eduroam be counted? 

* ID scanning system
  * Requires readers at each door of the auditorium
  * Setup and tear down between classes
  * Can be cost-prohibitive (pre-built kiosk)
  * Theft of hardware (custom-built laptop/scanner)



## Miscellanea 

- Privacy concerns are minimal

  > "We already violate [student] privacy by taking attendance" -- Alberto

  * Attendance taking is legit by [FERPA standards](https://www.cdc.gov/phlp/publications/topic/ferpa.html)
  * Could make app features opt-in for privacy-sensitive students

- Data for Registrar attendance usage only

  - Previously, SCANTRON quizzes were administered five times a semester
  - The analysis showed a positive correlation between student attendance and grades
    - Causation not established

- Registrar requires these data halfway or a third way through the semester

  - They want to see when each student may have participated in class
  - These data serve as a proxy for this requirement

  > "Just a list of students (names and/or IDs) and their attendance is enough" -- Alberto

- Further questions for Alberto can be directed to [Elizabeth](mailto:elizabeth-kleiman@uiowa.edu)

