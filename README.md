# Arshdeep Mann — Portfolio

Fourth-year Computer Science student at Simon Fraser University, seeking a co-op starting January 2027 in software development, data, or cloud.

[Email](mailto:asm32@sfu.ca) · [GitHub](https://github.com/arshmann2003) · New Westminster, BC

---

## Featured project

### Heart Disease Risk Screener
**Python · scikit-learn · pandas · Streamlit · GitHub Actions**
[Live demo](https://heart-risk-screener.streamlit.app/) · [Source](https://github.com/arshmann2003/HeartDiseaseClassifier)

A web app that estimates heart-disease risk from 21 health-survey answers, trained on 253,680 CDC survey records, and shows which answers drive each person's estimate.

- Found and fixed test-set leakage in threshold tuning, then rebuilt evaluation with separate training, validation, and test sets.
- The validated screening threshold catches 81% of cases at 2.6× the base-rate precision.
- Compared logistic regression, random forest, and tuned gradient boosting (0.85 ROC-AUC), selecting by PR-AUC because only 9% of records are positive, and kept predicted risks calibrated.
- K-Means clustering found a high-risk subgroup with a 5× higher heart-disease rate.
- Training and the app are packaged into tested Python modules, checked by CI on every push.

---

## Projects

### Student Performance Predictor
**Python · scikit-learn · pandas · Streamlit**
[Live demo](https://gpa-predictor-amann.streamlit.app/) · [Source](https://github.com/arshmann2003/student-performance-prediction)

An interactive app that predicts student GPA and exam scores, trained on 9,000 records from three public datasets. Models were benchmarked against a mean baseline. The GPA model reached R² 0.90, within 0.23 GPA points on average. Absences were the strongest predictor of GPA, far ahead of study time.

### Spring Maze
**Java · Spring Boot · JavaScript · HTML/CSS**
[Source](https://github.com/arshmann2003/mazeApp)

A browser maze game with a JavaScript frontend and a Spring Boot REST API that creates mazes, stores game state, and accepts each move. Work included fixing frontend–backend integration issues and documenting the API.

### Airlock Drop *(in progress)*
**Python · AWS S3 · Lambda · IAM**

A private file-drop service on AWS. Uploads stay in a private S3 bucket until a Lambda function checks size and file type. Files that pass get a short-lived presigned download link; files that fail are held for review and never served. IAM permissions are scoped so each part can touch only its own folder in the bucket.

### Library Management System
**Python · SQL · SQLite**

A Python application on a SQLite schema for members, loans, events, and staff tasks, with SQL for create, read, and update, and checks that records stay consistent after every action.

---

## Skills

| | |
|---|---|
| **Languages** | Python, Java, SQL, JavaScript, TypeScript, C, C++, R |
| **Data & ML** | pandas, NumPy, scikit-learn, matplotlib, Streamlit |
| **Web** | Spring Boot, REST APIs, HTML/CSS |
| **Cloud & tools** | AWS (S3, Lambda, IAM), Git, GitHub Actions, SQLite, Linux |

## Certifications

- AWS Certified Cloud Practitioner
- Google IT Support Professional Certificate

## Education

**B.Sc. Computer Science**, Simon Fraser University
Coursework: Algorithms, Systems Programming, Database Systems, Cybersecurity, Web Development, Computational Data Science

---

## About this site

A single static page: HTML, CSS, and a small JavaScript canvas animation. There is no build step and no server.

**Preview locally**

```bash
cd portfolio/website
python3 -m http.server 8088
```

Open http://127.0.0.1:8088

**Deploy to Amazon S3**

1. Create a bucket, turn on static website hosting with `index.html` as the index document, and allow public reads with a bucket policy for `s3:GetObject`.
2. Upload:

```bash
./deploy.sh your-bucket-name
```

3. For HTTPS, put a CloudFront distribution in front of the bucket. After each upload, refresh it:

```bash
aws cloudfront create-invalidation --distribution-id YOUR_ID --paths "/*"
```
