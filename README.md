# ThoracicSurgeryClassification

Овој проект споредува три модели на машинско учење (Logistic Regression, Random Forest и XGBoost) за предвидување дали пациентот ќе почине во рок од една година по извршената торакална операција.

Податочното множество е од UCI Machine Learning Repository и содржи информации за пациенти подложни на торакална хирургија. Се работи за бинарна класификација:

- **True** – пациентот починал во рок од една година по операцијата  
- **False** – пациентот преживеал

Карактеристики во множеството: Diagnosis, FVC, FEV1, Performance, Pain, Hemoptysis, Dyspnea, Cough, Weakness, Tumor size, Diabetes, MI, PAD, Smoker, Asthma, Age и Class.

Множеството е достапно на следниов линк: https://archive.ics.uci.edu/dataset/277/thoracic+surgery+data.

## Методи и резултати

- Моделите се тренираат со SMOTE за баланс на класи.
- Класичниот threshold од 0.5 беше намален на 0.3 за подобрување на recall кај ризичните пациенти.
- Random Forest и XGBoost покажаа најдобар баланс помеѓу recall и precision, додека Logistic Regression имаше највисок recall, но ниска AUC.
