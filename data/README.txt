Module 5 synthetic datasets

workshop_data.csv
- 200 observations
- Common dataset for the guided live workshop.

activity_data.csv
- Copy of Team 1 dataset for a default activity link.

activity_data_team_01.csv ... activity_data_team_10.csv
- Ten synthetic datasets for different teams.
- Sample sizes range from 158 to 247 observations.
- Same schema, but different underlying synthetic patterns/results.

Columns:
participant_id
group
hours
measurement_before
measurement_after

Suggested derived variable:
change = measurement_after - measurement_before

Suggested questions:
1. How many observations are there?
2. What is the mean baseline measurement?
3. What is the average change?
4. Is average change different between groups A and B?
5. Is hours associated with change?
6. What does a scatter plot suggest?
7. What can and cannot be concluded?

instructor_dataset_summary.csv
- Instructor-only quick reference with expected high-level patterns.
- Do not distribute this file to students if you want teams to discover the results independently.

All data are synthetic and should not be interpreted as observations from real participants or a real experiment.
