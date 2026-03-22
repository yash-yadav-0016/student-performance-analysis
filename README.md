# Student Academic Performance Analysis

## Project Overview

Comprehensive analysis of factors influencing student academic performance using correlation analysis, trend identification, and statistical testing across multiple courses.

**Objective:** Identify key factors that drive student academic success and provide actionable insights for performance improvement.

## Dataset

- **Records:** 500+ students
- **Courses:** 8 different courses (Mathematics, Physics, Chemistry, Biology, English, History, Economics, Computer Science)
- **Features:** 8 academic metrics
  - Attendance Rate (%)
  - Assignment Submission Rate (%)
  - Prior GPA
  - Study Hours Per Week
  - Participation Score (0-10)
  - Midterm Score (%)
  - Final Score (%)
  - Final GPA (Target)

## Methodology

### 1. Data Loading & Exploration
- Dataset overview and statistics
- Feature distribution analysis
- Missing value assessment

### 2. Exploratory Data Analysis (EDA)
- Descriptive statistics for all features
- Distribution analysis
- Initial pattern identification

### 3. Correlation Analysis
- Calculate correlations with Final GPA
- Identify strongest predictive factors
- Visualize relationships

### 4. Statistical Analysis
- Compare student groups (high/low performers)
- Analyze attendance impact
- Examine assignment submission effects
- Course-wise performance comparison

### 5. Trend Identification
- Segment students by performance level
- Identify success patterns
- Determine critical thresholds
- Find course difficulty variations

### 6. Visualizations
- Correlation heatmaps
- Scatter plots with trend lines
- Box plots by groups
- Course performance comparisons
- GPA distribution histograms

## Key Findings

### Top 3 Performance Drivers

1. **Attendance Rate** (0.7354 correlation) ⭐
   - Strongest single predictor of academic success
   - Students with <80% attendance: 2.83 avg GPA
   - Students with ≥80% attendance: 3.55 avg GPA
   - **Impact: 0.72 GPA points difference**

2. **Assignment Submission Rate** (0.5481 correlation)
   - Indicates consistent engagement
   - Students with <70% submission: 2.83 avg GPA
   - Students with ≥70% submission: 3.38 avg GPA
   - **Impact: 0.55 GPA points difference**

3. **Prior Course GPA** (0.2739 correlation)
   - Past performance predicts future success
   - Moderate but consistent indicator

### Critical Insights

✓ **Attendance Threshold:** Students with <80% attendance rarely achieve >3.0 GPA

✓ **Course Difficulty:** Performance varies by course
- Best Course: Economics (3.24 avg GPA)
- Challenging Course: Biology (3.02 avg GPA)

✓ **Success Pattern:** High attendance + regular assignments = 3.5+ GPA

✓ **Student Segments:**
- Excellent (GPA ≥ 3.5): 29.4% of students
- Average (2.5-3.5): 67% of students
- Struggling (< 2.0): 3.6% of students

✓ **Study Hours:** Less predictive than attendance/engagement (weak 0.05 correlation)

## Project Structure

```
student-performance-analysis/
├── README.md                              # Project documentation
├── requirements.txt                       # Python dependencies
├── student_performance_data.csv           # Dataset (500 records)
├── student_dataset.py                     # Dataset generation script
├── student_performance_analysis.py        # Main analysis script
├── student_performance_analysis.ipynb     # Interactive Jupyter notebook
├── student_performance_analysis.png       # Visualization plots
└── STUDENT_RESULTS_SUMMARY.txt           # Detailed results summary
```

## Technologies Used

**Programming Language:**
- Python 3.x

**Libraries:**
- **Pandas:** Data manipulation and analysis
- **NumPy:** Numerical computing
- **Matplotlib:** Static visualizations
- **Seaborn:** Statistical data visualization
- **SciPy:** Statistical testing

**Tools:**
- Jupyter Notebook for interactive analysis
- Git/GitHub for version control

## How to Run

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yash-yadav-0016/student-performance-analysis.git
cd student-performance-analysis
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

### Execution

#### Option 1: Run Python Script
```bash
python student_performance_analysis.py
```

This will:
- Load and analyze the dataset
- Perform correlation analysis
- Identify performance patterns
- Generate visualizations
- Display key findings

#### Option 2: Run Jupyter Notebook
```bash
jupyter notebook student_performance_analysis.ipynb
```

Interactive environment for:
- Step-by-step analysis
- Code modification
- Custom visualizations
- Detailed explanations

#### Option 3: Generate Dataset
```bash
python student_dataset.py
```

Creates a new synthetic dataset matching project specifications.

## Key Recommendations

### For Students
1. **Prioritize Attendance** - Strong predictor of success
2. **Submit Assignments Regularly** - Shows commitment and improves understanding
3. **Seek Help Early** - Particularly in challenging courses
4. **Consistent Study Habits** - Regular engagement beats cramming

### For Educators
1. **Monitor Attendance** - Intervene if students start missing classes
2. **Track Assignment Submission** - Early warning for struggling students
3. **Course-Specific Support** - Provide extra help in difficult courses
4. **Peer Mentoring** - Pair struggling students with high performers
5. **Early Intervention** - Identify at-risk students early

### For Administrators
1. **Attendance Policies** - Implement meaningful attendance expectations
2. **Assignment Deadlines** - Create accountability through regular deadlines
3. **Course Difficulty** - Balance course load and difficulty
4. **Support Services** - Provide tutoring in challenging courses

## Statistical Insights

### Correlation Strength
- **Strong:** Attendance (0.74)
- **Moderate:** Assignment Submission (0.55)
- **Weak:** Prior GPA (0.27), Study Hours (0.05)

### Performance Distribution
- **Mean GPA:** 3.12
- **Median GPA:** 3.14
- **Std Dev:** 0.58
- **Range:** 1.72 - 4.00

### Student Segments
- **Excellent (≥3.5):** 29.4% (147 students)
- **Average (2.5-3.5):** 67% (335 students)
- **Struggling (<2.0):** 3.6% (18 students)

## Limitations & Considerations

- Analysis based on 500 students; larger datasets may reveal additional patterns
- Course differences may be due to inherent difficulty or student selection
- Correlation doesn't imply causation (high attendance might correlate with motivation)
- External factors (mental health, socioeconomic) not captured in data
- Should be combined with qualitative feedback from students/teachers

## Future Improvements

- **Time-Series Analysis:** Track performance changes over semesters
- **Predictive Modeling:** Build ML models to predict future performance
- **Socioeconomic Factors:** Include demographics and background variables
- **Course Content Analysis:** Examine curriculum impact on performance
- **Intervention Analysis:** Measure impact of support programs
- **Causal Analysis:** Use causal inference to determine true drivers

## Author

**Yash Yadav**
- B.Tech CSE (Data Analytics Specialization) | UPES Dehradun
- GitHub: [github.com/yash-yadav-0016](https://github.com/yash-yadav-0016)
- LinkedIn: [linkedin.com/in/yash-yadav-b23b0b321](https://linkedin.com/in/yash-yadav-b23b0b321)
- Email: yash0016yadav@gmail.com

## References

- Educational Psychology: https://en.wikipedia.org/wiki/Educational_psychology
- Student Retention: https://www.edglossary.org/student-retention/
- Pandas Documentation: https://pandas.pydata.org/
- Matplotlib Documentation: https://matplotlib.org/

## License

This project is open source and available under the MIT License.

## Acknowledgments

- Dataset inspired by real educational performance data
- Analysis methodology based on educational research
- Visualization techniques from data science best practices

---

**Last Updated:** March 2026

For questions or collaboration, please reach out!
