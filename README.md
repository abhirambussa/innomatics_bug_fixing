# Note Making Application Debugging
## Overview
This repository contains the source code for a Note Making application developed using Python, Flask, and HTML. The purpose of this project was to identify and rectify several issues in the existing code through the debugging process.

## Bug Fixes
### Bug 1: GET Method in POST Request
To resolve this issue:

Change request.args.get("note") to request.form.get("note").
Ensure the inclusion of the GET request in the route method list in Flask code: @app.route('/', methods=["GET", "POST"]).
## Bug 2: Missing Submit Button
### To address this issue:

Add the appropriate code in the HTML file to include the submit button.
## Bug 3: First Item Showing as NONE
### To fix this issue:

Introduce a condition to add inputs to notes, preventing the registration of "NONE" values.
## Conclusion
In summary, the bug-fixing process involved corrections to the Flask route, HTML form, and implementation of validation checks. Notable changes include accommodating both GET and POST requests, specifying the method as POST in the HTML form, and ensuring non-empty notes are appended to the list.

Usage
Clone the repository: git clone [https://github.com/yourusername/repo.git](https://github.com/abhirambussa/innomatics_bug_fixing)
Navigate to the project directory: cd repo
Run the application: python app.py
