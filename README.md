
# HealthConnect Week 7 – Analytical Testing, KPI Validation & Dashboard Refinement

## HealthConnect Clinic Experience Lab

### Data Analytics Track

Week 7 focused on testing the accuracy, consistency and usefulness of the analytical outputs developed during the earlier stages of the HealthConnect Clinic Experience Lab.

Rather than repeating the earlier exploratory analysis, this stage focused on analytical validation, KPI reconciliation, dashboard testing, segmentation checks and refinement of the decision-support dashboard.

---

## Week 7 Objective

The main objective was to determine whether the important analytical outputs were:

- Accurate
- Consistent with the underlying dataset
- Correctly represented in Power BI
- Robust across relevant segments
- Useful for business decision-making

---

## Testing Approach

The Week 7 testing process covered four main areas:

1. KPI validation
2. Data-quality validation
3. Analytical finding validation
4. Power BI dashboard testing and refinement

The analytical results were compared against the underlying HealthConnect appointment dataset and independently calculated validation results.

---

## KPI Validation

The following core outputs were tested:

| KPI | Validated Result |
|---|---:|
| Appointment Records | 5,000 |
| No-Show Rate | 48.46% |
| Attendance Rate | 46.28% |
| Reminder Coverage | 72.68% |
| Repeat No-Show Rate | 55.41% |
| Average Booking Lead Time | 29.64 days |

The KPI calculations reconciled successfully with the independent validation results.

---

## Data Quality Testing

Important data-quality checks included:

- Appointment row count reconciliation
- Unique appointment ID validation
- Duplicate record checks
- Missing distance values
- Missing waiting-time values
- Reminder-channel missingness
- Booking and appointment date consistency
- Booking lead-day reconciliation
- Previous no-show consistency

The validation checks did not identify duplicate appointment IDs or invalid booking-date sequences.

---

## Analytical Validation

### Booking Lead Time

Booking lead time remained the strongest observed analytical signal tested during Week 7.

Observed no-show rates increased across the lead-time groups, from approximately 27.81% for appointments booked 0–7 days in advance to approximately 67.69% for appointments booked 46–60 days in advance.

This pattern remained in the same direction when tested separately among appointments with and without recorded reminders.

---

### Previous No-Show History

Previous no-show history remained an important supporting segmentation variable.

Records with no previous no-shows had an observed no-show rate of approximately 43.51%, while records with previous no-show history showed a higher observed rate.

The finding was retained as a useful risk-segmentation signal rather than being interpreted as a causal relationship.

---

### Reminder Status

Reminder status showed an observed difference in no-show rates:

- Reminder recorded: approximately 47.36%
- No reminder recorded: approximately 51.39%

This result was treated as an association rather than evidence that reminders directly caused improved attendance.

---

### Distance to Clinic

Distance also showed an observed attendance pattern.

The no-show rate was approximately 46.45% for appointments within 0–5 km compared with approximately 57.76% for appointments more than 20 km away.

This was interpreted as a supporting access-related signal requiring further investigation.

---

### Waiting Time

Waiting time showed very little separation between attended and no-show appointments.

Average waiting time was approximately:

- Attended: 24.29 minutes
- No-show: 24.20 minutes

Waiting time was therefore de-emphasised as a primary no-show intervention area.

---

## Dashboard Testing

The Power BI dashboard was tested using relevant filters and segment selections.

Tests included:

- Lead Time Group
- Previous No-Show History
- Reminder Status
- Distance Band
- Appointment Type
- Patient Status

The filtered dashboard outputs were checked against independently calculated results.

The tested filters reconciled with the expected analytical values.

---

## Dashboard Refinements

The following improvements were made as a result of testing:

### 1. KPI definitions were clarified

Important KPI definitions were made more explicit to reduce ambiguity between overall and non-cancelled appointment measures.

### 2. Lead-time groups were ordered chronologically

Lead-time categories were arranged according to their actual booking intervals rather than alphabetical order.

### 3. Missing distance values were handled explicitly

Missing distance records were represented using an `Unknown` category rather than being silently excluded from the analysis.

### 4. Reminder-channel blanks were interpreted correctly

Blank reminder channels were treated in the context of reminder status rather than being interpreted as a separate reminder channel.

### 5. Visual clutter was reduced

The dashboard was refined to focus attention on the most decision-relevant analytical outputs.

### 6. Association and causation were separated

Observed relationships were communicated as associations rather than causal effects unless causal evidence was available.

---

## Validated Business Insights

The Week 7 testing confirmed that:

1. Longer booking lead times are associated with higher observed no-show rates.
2. Previous no-show history provides useful risk segmentation.
3. Reminder status shows a smaller observed attendance association.
4. Distance provides a supporting access-related signal.
5. Waiting time does not appear to be a leading differentiator in the current dataset.

---

## Recommendations

HealthConnect should consider additional engagement for appointments booked substantially in advance, while monitoring the operational effectiveness of any intervention.

Previous no-show history can be considered when designing targeted appointment-support strategies, provided that the approach is monitored for unnecessary or inappropriate targeting.

Reminder recording should be improved so that the organisation can distinguish between genuine non-delivery and incomplete data capture.

Distance-related attendance differences should be investigated further to determine whether transport, timing or access barriers contribute to missed appointments.

Waiting time should remain a secondary analytical variable unless future modelling demonstrates meaningful incremental predictive value.

---

## Limitations

The analysis is observational and therefore does not establish causal relationships.

The dataset also contains some missing values, particularly for distance, waiting time and reminder channel.

Further modelling and operational testing are required before analytical findings are converted into implemented interventions.

---

## Week 8 Readiness

The validated Week 7 findings provide a stronger foundation for the final HealthConnect analytics dashboard and decision-support work.

Week 8 can therefore focus on final dashboard refinement, business interpretation, executive communication and integration of validated findings.

---

## Project Learning

Week 7 strengthened my understanding that data analytics is not only about finding patterns.

Reliable analytics requires:

- Validating calculations
- Testing assumptions
- Checking dashboard outputs
- Investigating inconsistencies
- Understanding missing data
- Testing findings across relevant segments
- Communicating limitations
- Translating validated evidence into useful decisions

---

## Author

Audrey

Data Analytics Track  
HealthConnect Clinic Experience Lab  
AnalystLab Africa
