# FashionDays Testing with Unittest Library

## Introduction
Welcome to the FashionDays Testing Project! In this project, I will be conducting comprehensive functional and non-functional tests on the FashionDays website using the powerful **unittest** testing framework.

## Purpose
The primary purpose of this project is to conduct a wide range of tests to ensure the robustness and quality of the FashionDays website. These tests include functional tests such as Smoke Testing, Sanity Testing, and Regression Testing, as well as non-functional tests like Performance Testing, Accessibility Testing, and SEO Testing. The goal is to identify and address ERRORS, BUGS, FAILURES, and provide recommendations for improvements.

## Project Structure
The project is structured as follows:

- `authentication_page` package:
  - `positive_authentication_tests`: Functional positive tests on the authentication page.
  - `negative_authentication_tests`: Functional negative tests on the authentication page.
  - `authentication_page_non_functional_tests`: Non-functional testing using Google Lighthouse testing tool.

- `main_page` package:
  - `positive_main_page_tests`: Functional positive tests on the main page.
  - `negative_main_page_tests`: Functional negative tests on the main page.
  - `main_page_non_functional_tests`: Non-functional testing using Google Lighthouse testing tool.

- `newsletter_functionality` package:
  - `positive_newsletter_tests`: Functional positive tests regarding the newsletter functionality.
  - `negative_newsletter_tests`: Functional negative tests regarding the newsletter functionality.

- `search_functionality` package:
  - `positive_search_functionality_tests`: Functional positive tests regarding the search functionality.
  - `negative_search_functionality_tests`: Functional negative tests regarding the search functionality.

- `reports` directory: Contains HTML reports generated by HTMLTestRunner and Google Lighthouse.
- `setup.py`: Contains classes for establishing 'setUp' and 'tearDown' methods.
- `suite.py`: Contains the test suite to run the entire project and generate an HTML report.
- `utility_methods.py`: Contains methods used throughout the project.

## Libraries Used
- unittest
- selenium
- pytest
- time
- subprocess
- os
- HtmlTestRunner (*If not installable via pip, search for 'html-testRunner' in Python packages*)

## Installation
To install the required libraries, use the following commands:
- `pip install selenium`
- `pip install pytest`
- `pip install html-testRunner`

If you encounter compatibility issues, you can try upgrading the libraries:
- `pip install selenium --upgrade`
- `pip install pytest --upgrade`
- `pip install html-testRunner --upgrade`

## Running the Project
- To run the entire project, execute the 'suite.py' file.
- To run specific tests, use the green arrow on the class or method you want to run.

## Known Issues and Recommendations
- Address performance and accessibility issues on the website.
- Implement a message for empty search input on the search bar.
- Fix the price filter issue for more accurate filtering: when setting the price filter, setting the drag and drop at the very end makes the filter to be set on 0 (in the code), but not visually, additionally, because selenium acts so fast while setting the drag and drop at 0, the visual price still remains at the max.

**REMINDER:** Some tests are tied to timed campaigns and promotions, so they might enter the 'except' state when these events expire.


