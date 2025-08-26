# Indian Kids Screen Time — EDA, Robustness Checks, and Logistic Regression

## Project Description
This project looks at daily screen time among Indian children and asks which factors are linked with exceeding the **2-hour guideline**.  
I ran exploratory summaries, group comparison tests (**Welch’s t-test** and **Mann–Whitney U**), and a simple **logistic regression**.  
**Robustness:** Both Welch and Mann–Whitney gave **consistent conclusions**.


## How to Install and Run the Project

1) **Clone the repository**  
Open your terminal/command prompt and run:
    
    git clone https://github.com/rinayaha/screentime_project.git
    cd screentime_project

2) **Install dependencies**
    
    pip install -r requirements.txt

3) **Run the notebook**
    
    jupyter notebook

Open `screentime.ipynb` and **Run All**.  
Make sure `Indian_Kids_Screen_Time.csv` is in the **same folder** as the notebook (or update the `PATH` variable in the notebook).


## How to Use the Project
- Run all cells in `screentime.ipynb` from top to bottom.
- You’ll see:
  - EDA (counts, simple group means)
  - **Chi-square** + **Cramér’s V** for categorical association
  - **Welch’s t-test** (main) and **Mann–Whitney U** (robustness) for group differences
  - **Logistic regression** with an **odds-ratio table**


## Key Results
Children who exceeded the limit averaged **4.82 hours/day**, while those who did not averaged **1.58 hours/day** — a gap of **more than three hours**.
- Statistical tests showed this difference is **highly significant** and represents a **large effect**.
- Logistic regression indicated that **age increases** the odds of exceeding, while a **higher educational-to-recreational ratio strongly decreases** the odds.
- **Gender** had a smaller effect.
- **Device type** and **urban/rural** status did **not** show clear associations.
- Overall, **age** and the **quality/mix of screen time** are stronger predictors than **device choice** or **location**.


## Limitations
- Cross-sectional snapshot (no cause effect)
- Self-reported measures (possible bias)
- Modest sample size (estimates can be unstable)
- Some important factors not observed (e.g. parental rules)


## Challenges & Future Work
- **Small dataset:** Collect more observations to stabilize estimates
- **Category cleanup:** Standardize device names and usage labels
- **More context:** If available, include basic household/school variables to reduce confusing


## Repository Link
**GitHub:** https://github.com/rinayaha/screentime_project
