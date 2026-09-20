# Data Quality Copilot

An AI-assisted data-quality workflow that profiles CSV datasets, detects common quality issues, and turns deterministic checks into understandable findings and recommendations.

## Workflow

```text
CSV Input → Data Profiling → Quality Checks → Issue Classification → AI-Assisted Explanation → Quality Report
```

## Quality Dimensions

- **Completeness:** missing values, null rates, empty fields
- **Consistency:** data-type and formatting inconsistencies
- **Uniqueness:** duplicate records
- **Validity:** invalid formats and constraint violations
- **Anomalies:** outliers and suspicious statistical patterns

## Key Capabilities

- Reads and profiles CSV datasets
- Calculates data-quality statistics
- Detects missing values, duplicates, formatting issues, and anomalies
- Uses AI to explain findings and suggest remediation
- Produces a reviewable quality report without modifying the source dataset

## Tech Stack

Python · pandas · OpenAI API · python-dotenv

## Run Locally

```bash
pip install -r requirements.txt
python data_copilot.py
```

Place CSV inputs in `data/`. A sample dataset is included for experimentation.

## Engineering Focus

The project intentionally separates **deterministic data validation** from **AI-assisted interpretation**. Quality metrics are calculated programmatically; the language model is used to make findings easier to understand and act on.

That separation is important for analytics and enterprise data workflows where measurable checks should not depend on probabilistic model output.

## Example Findings

```text
Missing-value rate detected in a required field
Duplicate records identified
Inconsistent date or text formats detected
Potential numeric outliers surfaced for review
```

## Roadmap

- Configurable validation rules
- Schema and threshold configuration
- Interactive data-quality dashboard
- Historical quality monitoring
- Automated tests
- API-based execution
- Exportable HTML/JSON reports

## Data Safety

The application is designed to analyze rather than automatically overwrite source data. Sensitive datasets should not be sent to external model providers without appropriate organizational approval and controls.
