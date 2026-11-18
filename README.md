<div align="center">

# 🎓 Student Success Prediction | توقع نجاح الطالب

**Predict whether a student will pass or fail using machine learning.**
**نتوقع نجاح الطالب أو رسوبه باستخدام التعلم الآلي.**

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-F7931E?logo=scikitlearn&logoColor=white)
![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-F37626?logo=jupyter&logoColor=white)
![Language](https://img.shields.io/badge/Language-العربية%20%7C%20English-6366f1)

</div>

---

## 🇬🇧 English

### About
This project builds a complete machine learning pipeline that predicts whether a student **passes (1)** or **fails (0)** based on weekly study hours, attendance rate, previous exam score, and city. It combines the work of Labs 1, 2 and 3 into one project.

### What the project does
1. **Explore** the data (shape, missing values, target distribution)
2. **Feature engineering**: creates `Effort_Index = Study_Hours × Attendance / 100`
3. **Train/Test split** with stratification
4. **Preprocessing pipeline**: median imputation + scaling for numbers, most-frequent imputation + One-Hot encoding for categories
5. **Train 3 models**: Logistic Regression, Random Forest, Gradient Boosting
6. **Hyperparameter tuning** with `GridSearchCV`
7. **Evaluate** using Accuracy, F1, ROC-AUC, PR-AUC and the confusion matrix
8. **Explain** the model with feature importance
9. **Predict** for a new student

### Results
| Model | Accuracy | F1 | ROC-AUC | PR-AUC |
|---|---|---|---|---|
| Logistic Regression | 0.85 | 0.87 | 0.96 | 0.97 |
| Random Forest | 0.80 | 0.83 | 0.86 | 0.90 |
| Gradient Boosting | 0.70 | 0.75 | 0.84 | 0.88 |

Most important feature: **Effort_Index**.

> ⚠️ The dataset is small (80 rows) and synthetic, so the results are for learning purposes only.

### Screenshots
| Target distribution | Model comparison |
|---|---|
| ![](images/target_distribution.png) | ![](images/model_comparison.png) |

| Confusion matrix | Feature importance |
|---|---|
| ![](images/confusion_matrix.png) | ![](images/feature_importance.png) |

### How to run
```bash
git clone https://github.com/YOUR_USERNAME/Student-Success-Prediction.git
cd Student-Success-Prediction
pip install -r requirements.txt
jupyter notebook Student_Success_Prediction.ipynb
```
Or upload the notebook to [Google Colab](https://colab.research.google.com) and run all cells.

### Project structure
```
Student-Success-Prediction/
├── Student_Success_Prediction.ipynb   # main code
├── requirements.txt                   # libraries
├── README.md                          # this file
└── images/                            # charts
```

---

## 🇸🇦 العربية

### عن المشروع
مشروع تعلم آلي كامل يتوقع هل الطالب **سينجح (1)** أو **سيرسب (0)** بناءً على ساعات المذاكرة الأسبوعية، ونسبة الحضور، ودرجته السابقة، ومدينته. المشروع يجمع أعمال المعامل الثلاثة (Lab 1, 2, 3) في مشروع واحد.

### خطوات المشروع
1. **استكشاف البيانات** (الحجم، القيم المفقودة، توزيع الهدف)
2. **هندسة الخصائص**: إنشاء خاصية `Effort_Index` = ساعات المذاكرة × نسبة الحضور ÷ 100
3. **تقسيم البيانات** إلى تدريب واختبار
4. **خط المعالجة**: تعويض القيم المفقودة وتوحيد المقاييس للأرقام، وترميز One-Hot للنصوص
5. **تدريب 3 نماذج**: Logistic Regression و Random Forest و Gradient Boosting
6. **تحسين الإعدادات** باستخدام `GridSearchCV`
7. **التقييم** بمقاييس Accuracy و F1 و ROC-AUC و PR-AUC ومصفوفة الالتباس
8. **تفسير النموذج** بأهمية الخصائص
9. **توقع** نتيجة طالب جديد

### النتائج
أفضل أداء على بيانات الاختبار كان لنموذج Logistic Regression، وأهم خاصية هي **Effort_Index**.

> ⚠️ البيانات صغيرة (80 سجل) ومولّدة للتعلم فقط، فالنتائج تعليمية.

### طريقة التشغيل
```bash
pip install -r requirements.txt
jupyter notebook Student_Success_Prediction.ipynb
```
أو ارفع الـ notebook على [Google Colab](https://colab.research.google.com) وشغّل كل الخلايا.

---

<div align="center">

**Author | الطالب:** YOUR_NAME · **ID | الهوية:** YOUR_ID
**Instructor | المعلمة:** أ. لطيفة سعد

</div>
