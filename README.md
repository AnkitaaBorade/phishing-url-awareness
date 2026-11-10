# Phishing URL Awareness Checker

## 1. Project Overview

The Phishing URL Awareness Checker is a Python-based command-line tool that checks URLs for common phishing warning signs. It helps users understand suspicious URL patterns and encourages safer browsing habits.

The program checks the URL text without opening or visiting any website.

## 2. Features

The tool checks for six warning signs:

1. Presence of the `@` symbol.
2. URL length greater than 100 characters.
3. IP address used as the hostname.
4. Five or more hostname segments.
5. Punycode marker (`xn--`).
6. Use of HTTP instead of HTTPS.

It displays all detected warning signs and provides a cautionary message when no listed warning signs are found.

## 3. Requirements

- Python 3.x
- No external Python packages required.

The project uses Python's built-in libraries.

## 4. How to Run

1. Open the project folder in VS Code.
2. Open the terminal.
3. Run the following command:

```bash
python phishing_checker.py
```

4. Enter a sample URL when prompted.
5. Type `q` to quit the program.

## 5. Example Output

**Input:**

```text
https://www.example.com/login
```

**Output:**

```text
Result:
- No listed warning signs found. This does NOT prove safety.
```

## 6. Testing

The program was tested using five sample URLs provided in the project workbook.

The test cases and actual results are documented in:

`tests/test_samples.md`

All five sample tests produced the expected results.

## 7. Screenshots

### Sample Run

![Sample Run](screenshots/sample_run.png)

### Test Results

![Test Results](screenshots/test_results.png)

## 8. Improvements Implemented

Two improvements were implemented:

- **Loop and Quit Option:** Users can check multiple URLs without restarting the program. They can type `q` to exit.
- **Malformed URL Handling:** The program handles malformed URL input without crashing.

## 9. Limitations

- The program only checks visible URL text.
- It does not open or visit websites.
- It does not scan for malware.
- It does not use online reputation services.
- It cannot guarantee whether a URL is safe or malicious.

## 10. Ethical Use

This project is intended for educational awareness. It helps users recognize common suspicious URL patterns. It should not be used to make final security decisions or to claim that a website is completely safe.

## 11. Author

- **Name:** Ankita Ajay Borade
- **Batch/Course:** Batch 1 , Ewb AI POWERED CYBERSECURITY INTERNSHIP
- **GitHub Username:** https://github.com/AnkitaaBorade/phishing-url-awareness