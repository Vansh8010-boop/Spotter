# Freight Rate Prediction Challenge

See `Freight_Rate_ML_Assessment.pdf` for the assessment instructions.

## What to do

1. Train and validate your model using `data/train_test.csv`.
2. Predict every load in `data/validation.csv`. Each load has a unique `load_id`.
3. Fill the matching `predicted_rate` values in `validation-predictions-template.csv` and save the result as `results/validation/validation_predictions.csv`.
4. Predict every row in `december-chart-inputs.csv` and save the completed file as `results/december/december_chart_inputs.csv`.
5. Install the scorer requirements and run:

```bash
python -m pip install -r requirements.txt
python score.py --predictions results/validation/validation_predictions.csv --december-predictions results/december/december_chart_inputs.csv
```

The scorer validates both files and creates `scorer_results/candidate_december.png`.

## Submit

- GitHub repository containing your code, dependencies, and run instructions
- `results/validation/validation_predictions.csv`
- `results/december/december_chart_inputs.csv`
- PDF or DOCX report containing your validation, data split approach and `candidate_december.png`
- 2-3 minute Loom link