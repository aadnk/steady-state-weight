## Steady-State Weight Calculator

Live demo: [Steady-State Weight Calculator](https://aadnk.github.io/steady-state-weight/)

### Purpose

This tool calculates the **steady-state weight** of an individual using the **Mifflin-St Jeor equation**, a widely used formula to estimate Basal Metabolic Rate (BMR). 

The steady-state weight is the weight you will naturally reach over time if:
1. You consistently consume a specified number of calories per day.
2. You maintain the same level of physical activity.

It helps users understand how caloric intake, age, height, sex, and activity level influence their steady-state weight.

---

### How It Works

The tool uses the **Mifflin-St Jeor equation**:

\[
\text{BMR} = 10W + 6.25H - 5A + S
\]

Where:
- \( W \) = Weight in kilograms (to be solved for steady state)
- \( H \) = Height in centimeters
- \( A \) = Age in years
- \( S \) = Gender constant (+5 for males, -161 for females)

To account for physical activity, the BMR is adjusted using an **exercise modifier**, which reflects the user's activity level. The equation is rearranged algebraically to solve for the steady-state weight where caloric intake matches the adjusted BMR.

---

### Features

1. **Dynamic Input**: The tool calculates the result automatically whenever an input field changes, as long as all fields are filled in.
2. **Persistence**: All inputs are saved locally using `localStorage`. When you revisit the tool, your previous inputs are automatically restored.
3. **User-Friendly Interface**: Simple design with clear instructions and interactive elements.
4. **Real-Time Results**: The calculated steady-state weight is displayed instantly.

---

### How to Use It

1. **Open the File**:
   - Save the provided HTML code as a file (e.g., `steady_state_calculator.html`) and open it in a modern web browser (Chrome, Firefox, Edge, etc.).

2. **Enter Inputs**:
   - Fill in the following details:
     - **Daily Calories**: The number of calories you consume per day.
     - **Height**: Your height in centimeters.
     - **Age**: Your age in years.
     - **Sex**: Select either "Male" or "Female".
     - **Exercise Modifier** (optional): Represents your activity level. The default is `1.15`, assuming light activity.

3. **View Results**:
   - The steady-state weight will update automatically as you fill in or modify any field.

4. **Revisit**:
   - All your inputs are saved automatically, so when you reload or revisit the page, the values will be pre-filled.

---

### Example

- **Daily Calories**: 2100 kcal  
- **Height**: 180 cm  
- **Age**: 35 years  
- **Sex**: Male  
- **Exercise Modifier**: 1.15  

**Result**: `87.11 kg`

This means that if you consistently consume **2100 kcal** per day and maintain a light activity level, your steady-state weight will be **87.11 kg**.

---

### Requirements

- A modern web browser (no internet connection needed).
- The HTML file.

---

### Notes

- Adjust the **Exercise Modifier** based on your activity level:
  - `1.2` = Sedentary (little or no exercise)
  - `1.375` = Lightly active (light exercise/sports 1-3 days a week)
  - `1.55` = Moderately active (moderate exercise/sports 3-5 days a week)
  - `1.725` = Very active (hard exercise/sports 6-7 days a week)
  - `1.9` = Extra active (very hard exercise, physical job, or twice-a-day training)
- The results are estimates and assume consistency in caloric intake and activity.

---

### Author

Kristian S. Stangeland

MIT License 
