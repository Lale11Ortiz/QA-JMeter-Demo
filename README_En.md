# QA-JMeter-Demo

Performance testing practice using Apache JMeter.
Simulates 10 concurrent users accessing the /posts endpoint from the public JSONPlaceholder API.
Includes HTML report, organized folder structure and CLI execution.

---

## 📌 Technical Summary

- 🔧 Tool: Apache JMeter 5.6.3
- 🌐 API: https://jsonplaceholder.typicode.com/posts
- 👥 Simulated users: 10
- 🔁 Loops per user: 1
- ⏱️ Ramp-Up: 5 seconds
- 📈 HTML report: Yes

---

## 📁 Project Structure

QA-JMeter-Demo/
  - test-plan.jmx          # JMeter test plan
  - evidences/             # .jtl results and screenshots
  - report/                # Auto-generated HTML report
  - README.md # (ESP)
  - README_En.md # (ENG)

---

## ▶️ How to run from CLI

```bash
jmeter -n -t test-plan.jmx -l evidences/results.jtl -e -o report/

---

## 📊 Sample Test Result

Total requests:     10
Duration:           6 seconds
Requests/sec:       1.8
Avg. response time: 545 ms
Error rate:         0.00%