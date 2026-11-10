# Test Results

Python version used: Python 3.13.1
Operating system: Windows
Date: 10 November 2026

| # | Input | Expected result | Actual result | Pass/Fail |
|---|-------|-----------------|---------------|-----------|
| 1 | https://www.example.com/login | No listed warning signs | No listed warning signs found | PASS |
| 2 | http://192.0.2.10/account     | IP address + HTTP | IP address warning + HTTP warning | PASS |
| 3 | http://example.com@sample.invalid/login | @ symbol + HTTP | @ symbol warning + HTTP warning | PASS |
| 4 | https://a.b.c.d.e.example.invalid/path  | Many hostname segments | Many hostname segments/subdomains warning | PASS |
| 5 | https://xn--example.invalid/  | Punycode-style hostname | Punycode-style hostname warning | PASS |

## Notes

All five sample URLs produced the expected warning results.
The program also handled blank input and malformed URL input without crashing.

