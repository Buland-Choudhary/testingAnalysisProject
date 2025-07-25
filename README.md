'''
# 🧪 Software Testing Analysis – Joda-Time

This project was developed as part of **CPEN 422 – Software Testing** at the University of British Columbia by **Buland Choudhary** and **Gurjas Singh Oberoi**. It demonstrates practical skills in automated test generation, coverage analysis, and evaluation using state-of-the-art tools and AI models.

## 📌 Project Overview

We chose the popular open-source Java library **[Joda-Time](https://github.com/JodaOrg/joda-time)** to evaluate and improve the test coverage of three key classes:

- `DateTimeUtils.java`
- `DateTimeZone.java`
- `Interval.java`

The goal was to compare **human-written**, **automatically generated**, and **AI-assisted** test suites in terms of **branch** and **line** coverage using **JaCoCo**, **EvoSuite**, **Randoop**, and **ChatGPT**.

---

## ⚙️ Tools and Technologies

- **Java**, **Maven**
- **JaCoCo** – Code coverage analysis
- **EvoSuite** – Automatic unit test generation
- **Randoop** – Random test generation
- **ChatGPT / GPT-4** – AI-assisted test creation
- **JUnit** – Unit testing framework

---

## 📊 Coverage Highlights
The value "xx/yy%" represent "xx%" line coverage and "yy%" branch coverage achieved.

| Class              | Human Tests | EvoSuite | Randoop | ChatGPT (Final Prompting) | Best Combined |
|-------------------|-------------|----------|---------|----------------------------|----------------|
| DateTimeUtils     | 92/93%      | 95/86%   | 82/69%  | 63/86%                     | **97/95%**     |
| DateTimeZone      | 89/85%      | 80/76%   | 61/52%  | 76/72%                     | **93/92%**     |
| Interval          | 94/95%      | 100/100% | 82/77%  | 44/37%                     | **100/100%**   |

> ✅ Combining human + automated + AI-generated tests significantly boosted overall coverage and test quality.

---

## 🤖 AI Testing Insights

Using **ChatGPT**, we experimented with various prompting strategies:

- Initial prompts with only class code resulted in low coverage.
- Including existing human tests improved results.
- Iterative feedback on test failures/coverage reports yielded the best outcomes (especially for `DateTimeZone`).

> ⚠️ For `Interval.java`, GPT-4 limitations in our free plan restricted test quality.

---

## 🧠 Key Takeaways

- **EvoSuite** achieved the best automated results across all classes, especially in branch coverage.
- **Randoop** produced many redundant or ineffective tests due to its random nature, but added slight value when time constraints were increased.
- **ChatGPT** showed promise in generating human-readable, adaptable tests, though coverage was variable.
- Manual and tool-assisted strategies **complement** each other well.

---

## 📁 Project Structure

- /src/main/java/org/joda/time/ # Target source classes
- /src/test/java/org/joda/time/ # Human-written + tool-generated tests
- /evosuite-tests/ # Tests by EvoSuite
- /randoop-tests/ # Randoop-generated regression tests
- /chatgpt-tests/ # AI-generated test suites
- jacoco-report/ # Final coverage reports
---

## 📈 Sample Workflow

1. **Set up** Joda-Time locally and integrated JaCoCo for coverage.
2. **Generated** tests using:
   - EvoSuite (via Maven plugin)
   - Randoop (manual configuration with time tuning)
   - ChatGPT (prompting via class descriptions, feedback)
3. **Analyzed** all results using JaCoCo HTML reports.
4. **Documented** the experiment with side-by-side comparison tables and analysis.

---

## 🎯 Skills Demonstrated

- Advanced test suite design and evaluation
- Proficient use of static/dynamic analysis tools
- Prompt engineering and feedback iteration for AI tools
- Maven and command-line workflow automation
- Detailed reporting, synthesis, and professional software communication

---

## 🙋‍♂️ Authors

- **Buland Choudhary** – [LinkedIn](https://linkedin.com/in/bulandchoudhary)
- **Gurjas Singh Oberoi**

---
'''
