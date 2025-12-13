# StudySaga - Final Project

## Project Summary
StudySaga is a C++ console application designed to streamline academic management. It utilizes the Standard Template Library (STL) to handle complex data relationships between Teachers, Students, Assignments, and Quizzes.

## Data Structures Used
* **std::vector (Dynamic Array):** Used for storing Assignments, Submissions, and Quizzes for fast random access.
* **std::unordered_map (Hash Table):** Used for the User Authentication system to provide fast O(1) login lookups.
* **std::set (Binary Search Tree):** Used to store student names for reporting, ensuring uniqueness and automatic alphabetical sorting.

## Key Features
1. **Polymorphic Auth System:** Supports both Teachers and Students via a base User class.
2. **Chronological Sorting:** Automatically sorts tasks by due date using operator overloading.
3. **File Persistence:** Saves user data to text files to prevent data loss.

## How to Run
1. Ensure `users.txt` exists in the directory.
2. Compile: `g++ main.cpp StudySystem.cpp -o StudySaga`
3. Run: `./StudySaga`
