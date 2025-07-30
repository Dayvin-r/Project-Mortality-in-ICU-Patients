# Project-Mortality-in-ICU-Patients

## I. Background
Many hospitals have an Intensive Care Unit (ICU) that provides care to the critically ill patients,
i.e., the patients that are in worst and most serious conditions. It is nowadays common for
healthcare providers to evaluate and report on the quality of patient care in a hospital, especially in
ICUs, to compare efficacy of medications, treatments, etc.
Hospitals usually cater very different patient cohorts, for example a community hospital, a tertiary
teaching hospital or a military hospital will have patients that may be of different age, gender,
different severity of illnesses, etc. So, in order for this reporting to be meaningful, it has to be riskadjusted, which means it controls for these different factors in the patient cohort. One way to do this
is to build a predictive model across all data from different hospitals for an outcome such as
mortality, length of stay, and readmission probability [3]. Then, such a predictive model can be used
as a benchmark, and hospitals/ICUs that underperform or outperform the benchmark can be
identified. Besides the benchmarking, such a predictive model can also be used to assess an
individual patient's risk.
To date, relatively simple models are common in this space, such as the Acute Physiology and
Chronic Health Evaluation (APACHE) score and its successors, the Australian and New Zealand
Risk of Death (ANZROD) model [4], and others. These models are usually linear models, based on
logistic regression or similar. Lately, it has been shown that Machine Learning (ML) models can
achieve more accurate predictions in this space [1, 2].

## II. Problem Statement
We work with data from the PhysioNet Computing in Cardiology Challenge 2012 [1, 2]. The
dataset contains 12,000 ICU stays, for which data from the first 48 hours of the ICU stay are
recorded. Up to 42 variables were recorded. There are 6 general descriptors, the other variables are
variables recorded potentially various times troughout the episode (time series), or just once, or not
at all. The goal is to develop, guided by the outcomes of the competition, a prototype for a Machine
Learning model that is able to predict the probability of death/survival.

## III. Main Objectives
This project aims to develop a model prototype that can predict mortality of ICU patients. This step
can be guided by the outcomes of the PhysioNet Challenge 2012 [1, 2]. 
