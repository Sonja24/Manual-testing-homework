Task Board Test Management and Issue Tracker - Test Execution Summary
Overview

This repository documents the results of our testing for the Task Board application. We tested two versions of the application (v.01 and v.02) to validate functionality, manage test cases, and track issues. Test cases were executed using TestRail, and any defects were logged in Jira.
Test Execution Summary
Task Board v.01

Application URL: Task Board v.01

In Task Board v.01, we performed extensive tests based on the SRS requirements. The focus was on verifying core functionalities and identifying bugs.
Key Test Areas:

    Authentication:
        Registration: Verified that users can register with valid data (unique email, password matching, etc.), and confirmed that redirection to the Home page occurs with the Logout button visible.
        Login & Logout: Ensured that login works correctly and that the Logout function returns the user to the Home page.

    Navigation:
        For logged-in users, navigation was checked to confirm that "Home," "Collection," "Search," "Create Book," and "Logout" were visible.
        For guests, only "Home," "Collection," "Search," "Login," and "Register" were displayed.

    CRUD Functionality:
        Book Creation: A book with a randomly generated title was created, ensuring uniqueness. All required fields (title, cover image, year, author, genre, and description) were filled and submitted.
        Book Editing and Deletion: The book was later edited and then deleted. Each operation was verified by checking the updated interface and URL.

Issues Identified:

Several defects were logged in Jira. Key issues included:

    Inconsistent form validation on the registration page.
    Navigation glitches under certain conditions.
    Minor discrepancies in CRUD operations.

Detailed bug reports—with reproduction steps, screenshots, and environment details—were submitted in Jira.
Task Board v.02

Application URL: Task Board v.02

After the development team addressed the reported issues, Task Board v.02 was tested to ensure all fixes were effective.
Key Test Areas:

    Regression Testing:
        All functionalities previously tested in v.01 were re-executed.
        Confirmed that critical issues had been resolved and that no new defects were introduced.
    Extended Functionality:
        Further tests were performed on navigation, authentication, and CRUD operations to ensure complete compliance with the SRS.

Outcomes:

    All major issues reported in Task Board v.01 were resolved.
    The application now meets the specified requirements.
    Minor issues observed did not affect the core functionality and were documented.

Test Artifacts

    TestRail:
    Detailed test cases and suites were created in TestRail covering authentication, navigation, and CRUD functionalities. These test cases include step-by-step procedures and expected outcomes.

    Jira:
    Bug reports for Task Board v.01 are available in Jira. Below is a summary:
        Bug #1: Registration form validation inconsistency – Resolved
        Bug #2: Navigation button display issues for logged-in users – Resolved
        Bug #3: CRUD operation glitches during book edit/delete – Resolved
        Additional issues were logged and reviewed as part of the regression process.

Conclusion

The testing process for the Task Board application was completed in two phases:

    Initial Testing (v.01): Identified and logged key issues.
    Re-Testing (v.02): Verified that bug fixes were effective and confirmed that the application meets the SRS requirements.
