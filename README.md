# ADS Audit: Assessing Performance and Fairness in Comment Toxicity Classification

## Background
The purpose of the Automated Decision System (ADS) is to effectively detect and classify toxic comments in online environments. The primary goals of this ADS are to ensure high accuracy in toxicity detection and minimize unintended model bias. This report aims to further analyze the ADS to maintain high accuracy performance while reducing biases related to identity attributes such as gender, race, sexual orientation, and disability. Achieving these goals presents challenges, especially the potential trade-off between accuracy and fairness. The audit evaluates the effectiveness of the ADS in managing these trade-offs through a critique of its bias reduction, validation process, and efficiency in evaluating toxicity assessment among demographic groups.

## Input and Output
The datasets include public comments sourced from the Civil Comments platform, curated by Jigsaw for the competition’s use. The output is a float score ranging from 0.0 to 1.0, with values larger or equal to 0.5 indicating a positive (toxic) label for accuracy evaluation. Data types, missing values, and distributions are analyzed for various features, along with correlations between features.

## Implementation and Validation
The ADS is implemented using an ensemble method combining predictions from multiple BERT models, along with an XLNet model and a GPT model, to assess toxicity. Performance is evaluated on both overall accuracy and sensitivity to demographic groups. Fairness metrics are employed to assess biases across different demographic groups.

## Outcomes
Key outcomes include high overall accuracy, precision, recall, and F1-score, indicating effective toxicity identification. However, disparities are evident among different demographic groups, suggesting potential biases. Stability analysis using the Population Stability Index (PSI) and evaluation of marginal cases highlight areas for improvement in model robustness and accuracy.

## Summary
The ADS shows promising accuracy but requires further calibration to minimize biases and enhance reliability across all groups. Potential improvements include oversampling/upweighting and considering alternative tokenizers. The ADS may be more suitable for deployment in the entertainment industry, but improvements are needed to ensure equitable treatment of users.

## Project Contribution
Contributions include research, exploratory data analysis, ADS implementation, data cleaning, evaluation of accuracy and fairness, stability analysis, and refinement of the report.

