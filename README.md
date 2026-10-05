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

**One-Variable Canonical Model**
- Slope (w): 8.621  
- Intercept (b): 55.18  
- R²: 0.9187  
- MSE: 28,827.8  

**- MODEL DIVERGE**


<img width="599" height="579" alt="Captura de pantalla 2026-10-05 145355" src="https://github.com/user-attachments/assets/b96afdd6-c60c-4a32-b239-29a51a7e57ad" />

**- DIVERGENCE WARNING**
<img width="584" height="562" alt="Captura de pantalla 2026-10-05 145412" src="https://github.com/user-attachments/assets/0e2e3ce1-7318-46b9-b3e6-29194f28d5ea" />


---
3. **Record the Canonical Model's slope, intercept, R², and MSE** from the One-Variable tab. Take a screenshot.
**
- Coeficients:  **
  - Size (m²): 8.15  
  - Bedrooms: 35.54  
  - Age (years): -9.27  
  - Distance to downtown (km): -14.29
 
   **- Intercept: **333.17  
**   - R²:** 0.9693  
**   - MSE:** 10,880.2


- COMBINATION 1
   - Bedrooms and Distance to downtown (km)
<img width="577" height="600" alt="Captura de pantalla 2026-10-05 145754" src="https://github.com/user-attachments/assets/c1505119-302b-401b-8ebc-8f7838924fec" />


- COMBINATION 2
   - Bedrooms and Age (years) 
<img width="581" height="647" alt="Captura de pantalla 2026-10-05 145844" src="https://github.com/user-attachments/assets/e2ce065f-e3ea-4b7b-8a58-4b4d17442c49" />


- ALL VARIABLES
   - Bedrooms, Age (years), and Distance to downtown (km) 
<img width="581" height="602" alt="Captura de pantalla 2026-10-05 145812" src="https://github.com/user-attachments/assets/77910a6f-c812-41b9-9ba2-823c299ac14a" />


---
4. **In the Multi-Variable tab, toggle features on and off in the playground** and watch R² change. Take a screenshot showing at least two different feature combinations and their R² values.

- Single-variable prediction (150 m²): 1,348.3 thousand MXN
<img width="350" height="110" alt="Captura de pantalla 2026-10-05 151511" src="https://github.com/user-attachments/assets/6de7b5d0-11f8-4352-bd23-9ad1bbace2f6" />

- Multi-variable prediction (150 m², 3 bedrooms, 5 years, 4 km): 1,559.3 MXM
<img width="518" height="115" alt="Captura de pantalla 2026-10-05 151551" src="https://github.com/user-attachments/assets/356f4faa-6b52-47b0-a031-b6494cbbe86d" />


---
5. **Record the Canonical (all 4 features) Model's coefficients, R², and MSE.** Take a screenshot.

The multivariable model is more accurate because it considers more factors (number of bedrooms, age, and distance), which improves the fit and reduces error.  
The single-variable model is simpler and faster to interpret, but it ignores important information.  
In real-world scenarios, real estate agencies use multivariable models to estimate more realistic prices, since a house's value depends not only on its size but also on its location and age.

6. **Use both canonical prediction tools** to predict the price of the **same house**: 150 m², 3 bedrooms, 5 years old, 4 km from downtown. Take a screenshot of both predictions.

<img width="409" height="133" alt="Captura de pantalla 2026-10-05 160636" src="https://github.com/user-attachments/assets/abe3e2cd-760f-4fcc-a45d-21a76d4ac9ec" />


7. **Fill out `A12_ReflectionQuestions.md`**, using the exact numbers from your Canonical Model screenshots, and submit it along with your labeled screenshots.
---
## Activity 12 — Reflection Questions: Mérida Homes

**1. Report the **Canonical One-Variable Model's** slope, intercept, R², and MSE.**

- The one-variable model uses only house size to predict price. With fixed parameters (learning rate = 0.3, iterations = 200), the canonical results are:

   - Slope (w): 8.621 → Each additional square meter increases the predicted price by about 8.6 thousand MXN.
   - Intercept (b): 55.18 → The baseline price when size is zero (a theoretical value).
   - R²: 0.9187 → The model explains about 91.9% of the variation in house prices.
   - MSE: 28,827.8 → The average squared error between predictions and actual prices, showing the model’s accuracy.

**2. Report the **Canonical Multi-Variable Model's** four coefficients (size, bedrooms, age, distance), intercept, R², and MSE.**

This model includes four features: size, bedrooms, age, and distance to downtown. With fixed parameters, the canonical results are:

- Coefficients:
   - Size (m²): 8.15 → Each square meter adds 8.15 thousand MXN.
   - Bedrooms: 35.54 → Each bedroom adds 35.5 thousand MXN.
   - Age (years): -9.27 → Each year of age reduces the price by 9.27 thousand MXN.
   - Distance (km): -14.29 → Each kilometer farther from downtown reduces the price by 14.3 thousand MXN.

- Intercept: 333.17 → The baseline value of the model.
- R²: 0.9693 → Explains 96.9% of the variation in prices, showing a stronger fit than the one-variable model.
- MSE: 10,880.2 → Much lower error, meaning the predictions are more precise.

**3. Which canonical model has the **higher R²** — one-variable or multi-variable — and what is the exact difference between the two R² values?**

- One-variable R² = 0.9187
- Multi-variable R² = 0.9693
- Difference = 0.0506  

The multi-variable model has the higher R², explaining about 5% more of the variation in prices compared to the one-variable model.

**4. Using the **Canonical One-Variable Model's** prediction tool, what is the predicted price for a 150 m², 3-bedroom, 5-year-old house located 4 km from downtown?**

- 1,348.3 thousand MXN  
This estimate is based only on size, ignoring bedrooms, age, and distance.

**5. Using the **Canonical Multi-Variable Model's** prediction tool, what is the predicted price for that exact same house?**

- 1,559.3 thousand MXN  
This higher estimate reflects the added value of bedrooms and adjusts for age and distance.

**6. Which canonical model predicts a **higher price** for that house, and what is the exact dollar (thousands of MXN) difference between the two predictions?**

- One-variable prediction: 1,348.3
- Multi-variable prediction: 1,559.3
- Difference = 211.0 thousand MXN  

The multi-variable model predicts a higher price, showing how additional features significantly influence valuation.

**7. In the Dataset tab, which single feature appears to have the **strongest visual relationship** with price?**

- From the scatter plots, size (m²) shows the strongest visual relationship with price. The points form a clear upward trend, making size the most predictive single feature.

**8. True or False: increasing the number of features used in a regression model can never *decrease* R² on the same training data it was fit on. Briefly justify your answer.**

- True.

On the same training dataset, adding more features cannot reduce R² because the model can always match or improve the fit. However, on new data (validation/test), R² can decrease due to overfitting, meaning the model fits the training data too closely and loses generalization ability.

9. In the One-Variable tab's playground, report **one learning rate** that caused the model to diverge (the warning appeared) and **one learning rate** that trained successfully (no warning).

- Divergent learning rate: 1.05 = The model failed to converge and displayed a divergence warning.
- Successful learning rate: 0.10 = The model trained correctly, producing a stable regression line without warnings.

---

# References:
- [Streamlit documentation](https://docs.streamlit.io/)
- [Markdown Guide](https://www.markdownguide.org/basic-syntax/)
