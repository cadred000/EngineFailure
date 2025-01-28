# Engine Failure Prediction Challenge

## Background
You are working with NASA turbofan engine degradation data. Your goal is to build a system that can predict when an engine will fail, allowing maintenance teams to optimize engine replacement and reduce both unnecessary maintenance and unexpected failures.

## Time Frame and Submission
- Submit as a public GitHub repository
- Use clear, descriptive commit messages throughout development
- Take up to two weeks to complete

## Dataset
You will be provided with run-to-failure data from turbofan engines:

- train_FD001.txt: Training data containing complete run-to-failure data
- test_FD001.txt: Test data that terminates sometime before failure
- RUL_FD001.txt: Ground truth Remaining Useful Life values for test data

Get data from here https://www.kaggle.com/datasets/behrad3d/nasa-cmaps

### Data Format
#### Training and Test Files (train_FD001.txt, test_FD001.txt)
Each row represents a snapshot during a single operational cycle:
- Column 1: Engine unit number
- Column 2: Time in cycles
- Columns 3-5: Operational settings
- Columns 6-26: Sensor measurements

#### RUL File (RUL_FD001.txt)
Single column containing the remaining useful life (in cycles) for each engine in the test set.

## Phase 1 (Required, 4-6 hours)

### 1. Data Processing & Feature Engineering (1-1.5 hours)
- Load and organize the datasets
- Create relevant time-based features
- Handle any anomalous values
- Normalize/standardize features as needed
- Analyze sensor degradation patterns

### 2. RUL Prediction Model (2-2.5 hours)
- Build a system to predict remaining useful life
- Requirements:
  * Must handle multivariate time series data
  * Should provide predictions with confidence intervals
  * Balance between early and late predictions
- You may use any modeling approach but must justify your choice

### 3. Model Evaluation & Documentation (1-1.5 hours)
- Create visualizations showing degradation patterns and predictions
- Document:
  * Model selection rationale
  * Feature engineering decisions
  * Performance metrics
  * Limitations and assumptions
- Include example of how system would be used in maintenance planning

### Deliverables
1. Python notebook containing:
   - Data processing pipeline
   - Model implementation
   - Evaluation metrics
   - Visualizations
2. Brief write-up (1-2 pages) explaining:
   - Approach taken
   - Key findings
   - Recommendations for implementation

## Phase 2 (Optional Extra Credit)

### Engine Health Monitoring Dashboard
Using any reporting engine of your choice (e.g., Plotly Dash, Streamlit), create:

1. Engine Health Overview
   - Current health status by engine
   - Historical degradation patterns
   - Sensor reading trends
   - Predicted RUL with confidence intervals

2. Maintenance Planning Tools
   - Prioritized list of engines needing maintenance
   - Risk assessment visualization
   - Maintenance schedule optimization
   - Cost impact analysis

3. Real-time Monitoring Interface
   - Live sensor data visualization
   - Early warning indicators
   - Historical comparison view
   - Configurable alert thresholds

### Bonus Features
- Interactive filtering capabilities
- Drill-down into individual sensor data
- Mobile-friendly views
- API endpoint for predictions
- Batch prediction capabilities

## Evaluation Criteria
- Code quality and documentation
- Feature engineering creativity
- Model performance (accuracy vs early/late predictions)
- Practical implementation considerations
- Clear communication of results
- For Phase 2: Dashboard usability and practical relevance

Note: While you may use AI tools for research and ideation, you'll need to demonstrate deep understanding of your implementation during technical interviews. Focus on building genuine comprehension of the techniques you employ.

There is no hard deadline, however there are limited positions available for this role and to some extent it's first come fist serve so if you take too long (many weeks) to complete the task you might find that there are not open positions left. Feel free to check with me if the posiition is still available.