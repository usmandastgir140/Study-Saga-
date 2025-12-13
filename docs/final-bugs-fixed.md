# Week 4 Bug Fix Log

1. **Date Sorting Error**
   * **Issue:** Assignments were not sorting correctly because the `operator<` was only comparing years, ignoring months and days.
   * **Fix:** Updated logic in `Models.h` to check Year -> then Month -> then Day.

2. **Duplicate Student Names in Report**
   * **Issue:** The quiz report listed the same student multiple times if they attempted a quiz twice.
   * **Fix:** Switched from `std::vector` to `std::set<string>` in `viewQuizMarks()` to automatically remove duplicates.

3. **File Parsing Crash**
   * **Issue:** The program crashed if `users.txt` had an empty line at the end.
   * **Fix:** Added a check `if (line.empty()) continue;` inside the file reading loop.
