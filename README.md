
Amazon Web Scraping Automation Suite
====================================

This project provides a solution for web scraping and automation testing of Amazon product pages using Playwright and Excel for easy data management.

Author: Aaryaman Gupta
Date: 15-Sep-2024
GitHub Repository: https://github.com/BoneyGupta/Amazon-Webscraping

--------------------------------------
Why Use This Automation Suite?
--------------------------------------

- This project simplifies automation for web scraping, monitoring, and testing with minimal code.
- The tool leverages Excel files for flow management and data visualization, making it accessible even for users without coding knowledge.
- Data is generated in logs and JSON files for easy reuse.
- The suite can handle both simple and complex automation scenarios with flexibility.

--------------------------------------
Building the Project:
--------------------------------------

1) Clone the repository to your desired directory:
   ```
   git clone git@github.com:BoneyGupta/Amazon-Webscraping.git
   ```

2) Install the required libraries:

   Prerequisites:
   - **Python 3.7 or later**: Check your Python version by running:
     ```
     python --version
     ```
   - **pip**: The Python package installer. Install it as per your operating system instructions:
     - Windows: [Download get-pip.py](https://bootstrap.pypa.io/get-pip.py)
     - macOS/Linux: Run the following command:
       ```
       python3 -m pip install --upgrade pip
       ```

   Install required libraries:
   ```
   pip install playwright openpyxl
   playwright install
   ```

3) Add the Chrome Application folder to your directory (if CDP is required):
   - Install Chrome Browser.
   - Copy the folder `C:\Program Files\Google\Chrome\Application` and add it to your project directory.
   - Open a command line terminal and run:
     ```
     chrome.exe --remote-debugging-port=9988 --user-data-dir=..\chromedata
     ```
   - Wait for the browser to open, then log in to the desired website.

4) Run the main program:
   ```
   python main.py
   ```

5) Enter the query when prompted.

6) View the reports in the `Reports` folder.

--------------------------------------
Running a Test:
--------------------------------------

1) Open the `Test.xlsx` file in the project directory.
2) Update the sheets with test cases. Refer to 'Template.xlsx' for examples.
3) Make sure to name the test sheets with the prefix 'test'.
4) Run the program to execute your test cases.

--------------------------------------
Features:
--------------------------------------

- Browser automation using Playwright (future plans for Selenium, API testing, and Appium).
- Results include logs, sequential data, and reference data in JSON format.
- Detailed test case structure for scraping product information from Amazon, including product title, rating, price, and features.

--------------------------------------
License:
--------------------------------------
This project is licensed under the MIT License.
