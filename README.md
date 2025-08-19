# Fitness & Exercise Data Preprocessing

This project processes multiple fitness and activity datasets into a **standardized format** for further analysis and machine learning. It cleans raw data, aligns columns across different sources, and exports updated CSV files with consistent schema.

---

## 📌 Features
- Standardizes multiple datasets into a common schema (`FINAL_COLUMNS`).
- Converts **height from BMI or meters → centimeters** for consistency.
- Maps generic exercise labels to meaningful categories (e.g., "Exercise 1" → Yoga).
- Creates **unique UserIDs** across datasets to avoid overlap.
- Outputs cleaned CSVs ready for downstream analysis.

---

## 📂 Input Datasets
The script expects the following CSV files in your Google Drive:

1. `Activity.csv`  
2. `dailyActivity_merged.csv`  
3. `exercise_dataset.csv`  
4. `gym_members_exercise_tracking.csv`  
5. `workout_fitness_tracker_data.csv`  

---

## 🏋️ Processed Outputs
The following cleaned datasets are generated:

- `UpdatedActivity.csv`
- `UpdatedDailyActivity.csv`
- `UpdatedExerciseDataset.csv`
- `UpdatedGymTracking.csv`
- `UpdatedWorkoutTracker.csv`

All outputs share the same schema:

| Column             | Description                                  |
|--------------------|----------------------------------------------|
| `UserID`           | Unique identifier for each user              |
| `exercise_name`    | Name of exercise (e.g., Running, Yoga)       |
| `exercise_type`    | Exercise category (Aerobic, Strength, etc.)  |
| `exercise_duration`| Duration in minutes                          |
| `age`              | Age of the user                              |
| `gender`           | Gender of the user                           |
| `weight`           | Weight in kilograms                          |
| `height`           | Height in centimeters                        |
| `heart_rate`       | Average heart rate (bpm)                     |
| `calories_burned`  | Calories burned during the session           |
| `bmi`              | Body Mass Index                              |

---

## ⚙️ Installation & Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/your-repo.git
   cd your-repo
