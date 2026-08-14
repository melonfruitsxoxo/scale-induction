# ML Club Selection: Track B

Everything you need for the Student Productivity Prediction task.

## What's here

```
data.csv                          1,500 student records
notebook/starter_notebook.ipynb   starter notebook
```

## Getting started

Clone the repo and open the notebook from inside the `notebook/` folder:

```bash
git clone <repo-url>
cd <repo-name>/notebook
jupyter notebook starter_notebook.ipynb
```

The notebook reads the data with `pd.read_csv('../data.csv')`, so it needs to stay
where it is for that path to work.

You'll need pandas, numpy, matplotlib, seaborn and scikit-learn.

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## The data

| Column                  | Meaning                                        |
| ----------------------- | ---------------------------------------------- |
| `age`                   | Student's age, 18 to 24                        |
| `study_hours_per_day`   | Average hours spent studying per day           |
| `sleep_hours`           | Average hours of sleep per night               |
| `phone_usage_hours`     | Hours spent on the phone daily                 |
| `social_media_hours`    | Hours spent specifically on social media daily |
| `attendance_percentage` | Class attendance as a percentage               |
| `stress_level`          | Self-reported stress, 1 to 10                  |
| `assignments_completed` | Number of assignments completed                |
| `productivity_score`    | The target. Overall productivity, 0 to 100     |

## Using the notebook

Run the setup cell first. It sets up two helpers you'll use throughout:

- `save_plot(name)` writes the current figure to `plots/<name>.png`. Use it instead of
  `plt.show()`, with the exact filenames each section asks for.
- `report_metrics(name, y_true, y_pred)` prints R2, MAE and RMSE in a consistent format
  and remembers them, so the comparison table in Section 6 builds itself.

The last cell checks that every plot we asked for actually exists before you submit.

You don't have to follow this structure. If you'd rather write it your own way, go ahead,
just keep the plot filenames the same so your submission is easy to read.

## Submitting

Three things:

- your notebook, with the outputs left in
- the `plots/` folder
- a one-page written report

Full task description, understanding checks and rubric are in the task document.
The submission link will be shared separately.
