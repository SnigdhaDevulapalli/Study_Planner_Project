# AI Based Study Planner (Java GUI)

## Overview

AI Based Study Planner is a simple Java desktop application that helps students organize their study time efficiently. The program allows users to add subjects, specify difficulty levels, track completed chapters, and automatically generate a study plan based on priority.

The application uses a basic AI-inspired priority algorithm to distribute available study hours among subjects.

## Features

* Add multiple subjects
* Define difficulty level (1–5)
* Track total and completed chapters
* Calculate pending chapters automatically
* Generate an AI-based study schedule
* Simple and interactive GUI using Java Swing

## Technologies Used

* Java
* Java Swing (GUI)
* AWT Event Handling
* Object Oriented Programming
* ArrayList Data Structure

## How the AI Logic Works

The study planner allocates time based on subject priority.

Priority is calculated using:

Priority = Difficulty × Pending Chapters

Where:

* Difficulty → Importance level of the subject (1 to 5)
* Pending Chapters → Remaining chapters to complete

Each subject receives study time proportional to its priority.

Allocated Time Formula:

Allocated Time = (Subject Priority / Total Priority of All Subjects) × Available Study Hours

This ensures difficult subjects with more pending chapters get more study time.

## Project Structure

StudyPlannerGUI.java

Contains:

* Subject class (data model)
* GUI interface
* Event handling
* AI-based time allocation logic

## How to Run the Project

1. Install Java (JDK 8 or higher)
2. Save the file as:

StudyPlannerGUI.java

3. Compile the program:

javac StudyPlannerGUI.java

4. Run the program:

java StudyPlannerGUI

## How to Use the Application

Step 1: Enter subject details

* Subject Name
* Difficulty (1–5)
* Total Chapters
* Completed Chapters

Step 2: Click **Add Subject**

Step 3: Enter available study hours for the day

Step 4: Click **Generate Plan**

The system will display a personalized study schedule.

## Example

Subject: Data Structures
Difficulty: 5
Total Chapters: 10
Completed: 4

Pending Chapters = 6

If total study time = 5 hours, the AI distributes hours based on priority compared to other subjects.

## Future Improvements

* Add subject editing and deletion
* Save study plans to a file
* Graphical progress tracking
* Daily and weekly scheduling
* Smarter AI recommendations
* Dark mode UI

## Author

Developed as a Java GUI project for learning AI-based scheduling concepts and Swing programming.
