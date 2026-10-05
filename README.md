# Activity 12: Mérida Homes — Predicting Property Prices
## Sessions 20, 21
## Due date (mm/dd/yyyy): 10/11/2026
## Adriana Rosales Gonzalez
## Delivery Format: [] Video URL | [X] Markdown file | [] Jupyter Notebook file

---
## The Story

**Mérida Homes** is a fictional real-estate agency. Before listing a property, agents want a quick, data-driven price estimate — a job perfectly suited to **Linear Regression**: learning a
straight-line (or flat-plane) relationship between a house's features and its price, from 60 real past sales.
---

### Your Tasks
1. **Read the Dataset tab.** Note which feature looks most strongly related to price just from
   the scatter plots.

2. **In the One-Variable tab, try at least 3 different learning rates in the playground**, including one large enough to make the model diverge. Take a screenshot of the divergence
   warning.

- MODEL DIVERGE
<img width="599" height="579" alt="Captura de pantalla 2026-10-05 145355" src="https://github.com/user-attachments/assets/b96afdd6-c60c-4a32-b239-29a51a7e57ad" />


- DIVERGENCE WARNING
<img width="584" height="562" alt="Captura de pantalla 2026-10-05 145412" src="https://github.com/user-attachments/assets/0e2e3ce1-7318-46b9-b3e6-29194f28d5ea" />


---
3. **Record the Canonical Model's slope, intercept, R², and MSE** from the One-Variable tab. Take a screenshot.

- COMBINATION 1
<img width="577" height="600" alt="Captura de pantalla 2026-10-05 145754" src="https://github.com/user-attachments/assets/c1505119-302b-401b-8ebc-8f7838924fec" />



- COMBINATION 2
<img width="581" height="647" alt="Captura de pantalla 2026-10-05 145844" src="https://github.com/user-attachments/assets/e2ce065f-e3ea-4b7b-8a58-4b4d17442c49" />



- COMBINATION 3
<img width="558" height="598" alt="Captura de pantalla 2026-10-05 145735" src="https://github.com/user-attachments/assets/48f4683c-2acb-4fdb-a409-d9722ac71eca" />



- ALL VARIABLES
<img width="581" height="602" alt="Captura de pantalla 2026-10-05 145812" src="https://github.com/user-attachments/assets/77910a6f-c812-41b9-9ba2-823c299ac14a" />


---
4. **In the Multi-Variable tab, toggle features on and off in the playground** and watch R² change. Take a screenshot showing at least two different feature combinations and their R² values.

- Single-variable prediction (150 m²): 1,348.3 thousand MXN
<img width="350" height="110" alt="Captura de pantalla 2026-10-05 151511" src="https://github.com/user-attachments/assets/6de7b5d0-11f8-4352-bd23-9ad1bbace2f6" />

- Multi-variable prediction (150 m², 3 bedrooms, 5 years, 4 km): 1,559.3 MXM
<img width="518" height="115" alt="Captura de pantalla 2026-10-05 151551" src="https://github.com/user-attachments/assets/356f4faa-6b52-47b0-a031-b6494cbbe86d" />



---
5. **Record the Canonical (all 4 features) Model's coefficients, R², and MSE.** Take a screenshot.

6. **Use both canonical prediction tools** to predict the price of the **same house**: 150 m², 3 bedrooms, 5 years old, 4 km from downtown. Take a screenshot of both predictions.

7. **Fill out `A12_ReflectionQuestions.md`**, using the exact numbers from your Canonical Model screenshots, and submit it along with your labeled screenshots.
---


# References:
- [Streamlit documentation](https://docs.streamlit.io/)
- [Markdown Guide](https://www.markdownguide.org/basic-syntax/)
