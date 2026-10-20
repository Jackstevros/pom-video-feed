# POM medical sources

Every question POM's **Ask your doctor** feature can show, when it is asked, and the published guideline,
study or reference behind it, with the exact claim POM takes from each source.

- POM prepares questions to bring to a clinician. It never recommends a test, treatment, medication or dose.
- Questions come from a fixed, reviewed rules table. No AI writes or rewords them.
- A source not re-reviewed within 365 days is withheld in the app until it is.
- New publications are checked monthly; changes are made only after review.

Rules version **2026.10.20.4** · 34 questions · 20 sources · machine-readable: [sources.json](sources.json)

_Not medical advice. Discuss any result with your clinician._

## Cholesterol

### My LDL-C was [your result], at or above 190 mg/dL. Should we check for secondary causes or familial hypercholesterolemia, and does this need a specialist?

- **Asked when:** LDL-C is 190 mg/dL or higher.
- **Rule:** `lipids.ldl.190`
- **Why:** Treats LDL-C of 190 mg/dL or higher as severe hypercholesterolemia, with evaluation for secondary causes and familial hypercholesterolemia. — [Blumenthal RS, Morris PB, Gaudino M, et al. 2026 ACC/AHA/AACVPR/ABC/ACPM/ADA/AGS/APhA/ASPC/NLA/PCNA Guideline on the Management of Dyslipidemia. Circulation. 2026. doi:10.1161/CIR.0000000000001423](https://doi.org/10.1161/CIR.0000000000001423)

### My LDL-C was [your result]. Is it persistently 160 mg/dL or higher, and should we recheck it to confirm?

- **Asked when:** LDL-C is 160–189 mg/dL.
- **Rule:** `lipids.ldl.160.persistent`
- **Why:** Lists persistently elevated LDL-C of 160 mg/dL or higher as a risk-enhancing factor; one result does not show persistence. — [Blumenthal RS, Morris PB, Gaudino M, et al. 2026 ACC/AHA/AACVPR/ABC/ACPM/ADA/AGS/APhA/ASPC/NLA/PCNA Guideline on the Management of Dyslipidemia. Circulation. 2026. doi:10.1161/CIR.0000000000001423](https://doi.org/10.1161/CIR.0000000000001423)

### My non-HDL cholesterol was [your result]. Should non-HDL be one of the goals we track alongside LDL?

- **Asked when:** Non-HDL cholesterol is flagged by the lab.
- **Rule:** `lipids.non_hdl.goal`
- **Why:** Sets treatment goals for both LDL-C and non-HDL-C, with lower goals for higher-risk groups. — [Blumenthal RS, Morris PB, Gaudino M, et al. 2026 ACC/AHA/AACVPR/ABC/ACPM/ADA/AGS/APhA/ASPC/NLA/PCNA Guideline on the Management of Dyslipidemia. Circulation. 2026. doi:10.1161/CIR.0000000000001423](https://doi.org/10.1161/CIR.0000000000001423)

### My triglycerides were [your result], at or above 500 mg/dL. Does this need prompt follow-up, and was it a fasting sample?

- **Asked when:** Triglycerides are 500 mg/dL or higher.
- **Rule:** `lipids.tg.500`
- **Why:** Treats fasting triglycerides of 500 mg/dL or higher as a marked elevation that needs evaluation. — [Blumenthal RS, Morris PB, Gaudino M, et al. 2026 ACC/AHA/AACVPR/ABC/ACPM/ADA/AGS/APhA/ASPC/NLA/PCNA Guideline on the Management of Dyslipidemia. Circulation. 2026. doi:10.1161/CIR.0000000000001423](https://doi.org/10.1161/CIR.0000000000001423)

### My triglycerides were [your result]. Was this a fasting sample, and should it be repeated fasting to confirm?

- **Asked when:** Triglycerides are 150–499 mg/dL.
- **Rule:** `lipids.tg.fasting`
- **Why:** Lists persistently elevated fasting triglycerides of 150 mg/dL or higher as a risk-enhancing factor; non-fasting results are interpreted differently. — [Blumenthal RS, Morris PB, Gaudino M, et al. 2026 ACC/AHA/AACVPR/ABC/ACPM/ADA/AGS/APhA/ASPC/NLA/PCNA Guideline on the Management of Dyslipidemia. Circulation. 2026. doi:10.1161/CIR.0000000000001423](https://doi.org/10.1161/CIR.0000000000001423)

### Can we estimate my 10-year cardiovascular risk (for example with the PREVENT calculator) using my cholesterol, HDL, blood pressure and other factors, and what does it mean for next steps?

- **Asked when:** Any cholesterol result is flagged (asked once per panel).
- **Rule:** `lipids.panel.risk_estimate`
- **Why:** Uses estimated 10-year risk (PREVENT) to place adults in risk groups such as borderline or intermediate, which guide next steps. — [Blumenthal RS, Morris PB, Gaudino M, et al. 2026 ACC/AHA/AACVPR/ABC/ACPM/ADA/AGS/APhA/ASPC/NLA/PCNA Guideline on the Management of Dyslipidemia. Circulation. 2026. doi:10.1161/CIR.0000000000001423](https://doi.org/10.1161/CIR.0000000000001423)
- **Why:** PREVENT estimates 10-year cardiovascular risk from factors including cholesterol, HDL cholesterol, blood pressure, diabetes, smoking and kidney function. — [Khan SS, Matsushita K, Sang Y, et al. Development and validation of the American Heart Association's PREVENT equations. Circulation. 2024;149:430-449. doi:10.1161/CIRCULATIONAHA.123.067626](https://doi.org/10.1161/CIRCULATIONAHA.123.067626)

### I have no Lp(a) result on record. Should I have Lp(a) measured once?

- **Asked when:** Any cholesterol result is flagged and no Lp(a) result is on record.
- **Rule:** `lipids.lpa.once`
- **Why:** Recommends measuring Lp(a) at least once in adulthood (Class 1). — [Blumenthal RS, Morris PB, Gaudino M, et al. 2026 ACC/AHA/AACVPR/ABC/ACPM/ADA/AGS/APhA/ASPC/NLA/PCNA Guideline on the Management of Dyslipidemia. Circulation. 2026. doi:10.1161/CIR.0000000000001423](https://doi.org/10.1161/CIR.0000000000001423)
- **Why:** Recommends that every adult has Lp(a) measured at least once. — [Kronenberg F, Mora S, Stroes ESG, et al. Lipoprotein(a) in atherosclerotic cardiovascular disease and aortic stenosis: a European Atherosclerosis Society consensus statement. Eur Heart J. 2022. doi:10.1093/eurheartj/ehac361](https://doi.org/10.1093/eurheartj/ehac361)

### Would an ApoB test add useful information alongside my cholesterol results?

- **Asked when:** Any cholesterol result is flagged and no ApoB result is on record.
- **Rule:** `lipids.apob`
- **Why:** Supports selective ApoB measurement to assess residual risk, for example with high triglycerides, metabolic syndrome or diabetes. — [Blumenthal RS, Morris PB, Gaudino M, et al. 2026 ACC/AHA/AACVPR/ABC/ACPM/ADA/AGS/APhA/ASPC/NLA/PCNA Guideline on the Management of Dyslipidemia. Circulation. 2026. doi:10.1161/CIR.0000000000001423](https://doi.org/10.1161/CIR.0000000000001423)
- **Why:** Reviews evidence that ApoB, a count of atherogenic particles, can capture risk that LDL-C alone misses. — [Sniderman AD, Thanassoulis G, Glavinovic T, et al. Apolipoprotein B particles and cardiovascular disease: a narrative review. JAMA Cardiol. 2019;4(12):1287-1295. doi:10.1001/jamacardio.2019.3780](https://doi.org/10.1001/jamacardio.2019.3780)

### If my 10-year cardiovascular risk is borderline or intermediate, would a coronary artery calcium (CAC) scan help us decide next steps?

- **Asked when:** Any cholesterol result is flagged, age 40–75 at the test, and no previous calcium scan.
- **Rule:** `lipids.cac`
- **Why:** Supports considering CAC scoring to reclassify risk in adults at borderline or intermediate risk when the decision is uncertain. — [Blumenthal RS, Morris PB, Gaudino M, et al. 2026 ACC/AHA/AACVPR/ABC/ACPM/ADA/AGS/APhA/ASPC/NLA/PCNA Guideline on the Management of Dyslipidemia. Circulation. 2026. doi:10.1161/CIR.0000000000001423](https://doi.org/10.1161/CIR.0000000000001423)
- **Why:** In MESA, CAC was strongly and gradedly associated with 10-year ASCVD events, independent of standard risk factors. — [Budoff MJ, Young R, Burke G, et al. Ten-year association of coronary artery calcium with atherosclerotic cardiovascular disease (ASCVD) events: the Multi-Ethnic Study of Atherosclerosis (MESA). Eur Heart J. 2018;39(25):2401-2408. doi:10.1093/eurheartj/ehy217](https://doi.org/10.1093/eurheartj/ehy217)

## Blood sugar

### My A1c was [your result], in the range the ADA uses for diabetes. Should it be confirmed with a repeat test?

- **Asked when:** A1c is 6.5% or higher.
- **Rule:** `glucose.a1c.diabetes`
- **Why:** Treats an A1C of 6.5% or higher as meeting a diabetes criterion; without clear symptoms it usually needs confirming with a second test. — [American Diabetes Association Professional Practice Committee. 2. Diagnosis and Classification of Diabetes: Standards of Care in Diabetes—2026. Diabetes Care. 2026;49(Suppl 1):S27. doi:10.2337/dc26-S002](https://doi.org/10.2337/dc26-s002)

### My A1c was [your result], in the range the ADA calls prediabetes. Should we recheck it, and how often should I be tested?

- **Asked when:** A1c is 5.7–6.4%.
- **Rule:** `glucose.a1c.prediabetes`
- **Why:** Treats an A1C of 5.7–6.4% as the prediabetes range; one result is not a diagnosis. — [American Diabetes Association Professional Practice Committee. 2. Diagnosis and Classification of Diabetes: Standards of Care in Diabetes—2026. Diabetes Care. 2026;49(Suppl 1):S27. doi:10.2337/dc26-S002](https://doi.org/10.2337/dc26-s002)
- **Why:** Recommends screening adults 35 to 70 with overweight or obesity, and suggests every 3 years may be reasonable when results are normal. — [US Preventive Services Task Force. Screening for Prediabetes and Type 2 Diabetes: US Preventive Services Task Force Recommendation Statement. JAMA. 2021. doi:10.1001/jama.2021.12531](https://www.uspreventiveservicestaskforce.org/uspstf/recommendation/screening-for-prediabetes-and-type-2-diabetes)

### My fasting glucose was [your result], in the range the ADA uses for diabetes. Should it be confirmed with a repeat test?

- **Asked when:** Glucose is 126 mg/dL or higher and the sample is documented as fasting.
- **Rule:** `glucose.fasting.diabetes`
- **Why:** Uses fasting plasma glucose of 126 mg/dL or higher, after at least 8 hours without calories, as a diabetes criterion that usually needs confirming. — [American Diabetes Association Professional Practice Committee. 2. Diagnosis and Classification of Diabetes: Standards of Care in Diabetes—2026. Diabetes Care. 2026;49(Suppl 1):S27. doi:10.2337/dc26-S002](https://doi.org/10.2337/dc26-s002)

### My fasting glucose was [your result], in the range the ADA calls prediabetes. Should we recheck it?

- **Asked when:** Glucose is 100–125 mg/dL and the sample is documented as fasting.
- **Rule:** `glucose.fasting.prediabetes`
- **Why:** Uses fasting plasma glucose of 100–125 mg/dL, after at least 8 hours without calories, as the prediabetes range. — [American Diabetes Association Professional Practice Committee. 2. Diagnosis and Classification of Diabetes: Standards of Care in Diabetes—2026. Diabetes Care. 2026;49(Suppl 1):S27. doi:10.2337/dc26-S002](https://doi.org/10.2337/dc26-s002)

### My glucose was [your result]. Was this a fasting sample? If not, should it be repeated fasting, or checked with an A1c?

- **Asked when:** Glucose is flagged and fasting is not documented.
- **Rule:** `glucose.fasting.unknown`
- **Why:** Applies its fasting glucose thresholds only after at least 8 hours without calories; other glucose tests are interpreted differently. — [American Diabetes Association Professional Practice Committee. 2. Diagnosis and Classification of Diabetes: Standards of Care in Diabetes—2026. Diabetes Care. 2026;49(Suppl 1):S27. doi:10.2337/dc26-S002](https://doi.org/10.2337/dc26-s002)

### Would a structured lifestyle program, such as a Diabetes Prevention Program, be right for me?

- **Asked when:** A1c or fasting glucose is in the prediabetes range (asked once).
- **Rule:** `glucose.panel.prevention`
- **Why:** Says people with prediabetes should be offered or referred to effective preventive interventions, such as lifestyle programs focused on diet and physical activity. — [US Preventive Services Task Force. Screening for Prediabetes and Type 2 Diabetes: US Preventive Services Task Force Recommendation Statement. JAMA. 2021. doi:10.1001/jama.2021.12531](https://www.uspreventiveservicestaskforce.org/uspstf/recommendation/screening-for-prediabetes-and-type-2-diabetes)
- **Why:** In adults at high risk, a structured lifestyle program reduced new cases of type 2 diabetes by 58% compared with placebo. — [Diabetes Prevention Program Research Group. Reduction in the incidence of type 2 diabetes with lifestyle intervention or metformin. N Engl J Med. 2002;346(6):393-403. doi:10.1056/NEJMoa012512](https://doi.org/10.1056/NEJMoa012512)

### Could anything make my A1c less accurate for me, such as anemia, recent blood loss or a hemoglobin variant?

- **Asked when:** A1c is flagged (asked once).
- **Rule:** `glucose.panel.a1c_accuracy`
- **Why:** Notes that A1C may be unreliable with some hemoglobin variants, altered red-cell turnover (for example anemia or blood loss) or certain therapies. — [American Diabetes Association Professional Practice Committee. 2. Diagnosis and Classification of Diabetes: Standards of Care in Diabetes—2026. Diabetes Care. 2026;49(Suppl 1):S27. doi:10.2337/dc26-S002](https://doi.org/10.2337/dc26-s002)

## Kidney

### Should my kidney tests be repeated to see whether this lasts 3 months or more, rather than reading one result?

- **Asked when:** Any kidney result is flagged (asked once; names an eGFR below 60).
- **Rule:** `kidney.panel.confirm`
- **Why:** Advises repeating tests after an unexpected abnormal result and not assuming kidney disease from a single eGFR or albumin value; chronic kidney disease needs at least 3 months, and an eGFR below 60 is flagged as low. — [Kidney Disease: Improving Global Outcomes (KDIGO) CKD Work Group. KDIGO 2024 Clinical Practice Guideline for the Evaluation and Management of Chronic Kidney Disease. Kidney Int. 2024;105(4S):S117-S314.](https://kdigo.org/wp-content/uploads/2026/05/KDIGO-2024-CKD-Guideline-Summary-Recommendations-and-Practice-Points.pdf)

### Should I have a urine albumin-to-creatinine ratio (uACR) test along with my eGFR?

- **Asked when:** Any kidney result is flagged and no urine albumin (uACR) is on record.
- **Rule:** `kidney.panel.uacr`
- **Why:** Recommends testing both urine albumin and estimated GFR in people at risk for, or with, chronic kidney disease. — [Kidney Disease: Improving Global Outcomes (KDIGO) CKD Work Group. KDIGO 2024 Clinical Practice Guideline for the Evaluation and Management of Chronic Kidney Disease. Kidney Int. 2024;105(4S):S117-S314.](https://kdigo.org/wp-content/uploads/2026/05/KDIGO-2024-CKD-Guideline-Summary-Recommendations-and-Practice-Points.pdf)

### Could my muscle mass, diet or recent hard training have affected my creatinine-based eGFR, and would a cystatin C test give a more accurate estimate?

- **Asked when:** Creatinine or eGFR is flagged and no cystatin C is on record.
- **Rule:** `kidney.panel.cystatin`
- **Why:** Notes creatinine is affected by muscle mass, exercise and diet, and recommends adding cystatin C (eGFRcr-cys) when the creatinine estimate is less accurate and the result matters for decisions. — [Kidney Disease: Improving Global Outcomes (KDIGO) CKD Work Group. KDIGO 2024 Clinical Practice Guideline for the Evaluation and Management of Chronic Kidney Disease. Kidney Int. 2024;105(4S):S117-S314.](https://kdigo.org/wp-content/uploads/2026/05/KDIGO-2024-CKD-Guideline-Summary-Recommendations-and-Practice-Points.pdf)

## Liver

### Should my liver tests be repeated to confirm, and if they stay raised, what evaluation makes sense?

- **Asked when:** ALT, AST or alkaline phosphatase is flagged (asked once).
- **Rule:** `liver.panel.repeat`
- **Why:** Recommends repeating the liver panel or doing a clarifying test to confirm an abnormal result before further evaluation. — [Kwo PY, Cohen SM, Lim JK. ACG Clinical Guideline: Evaluation of Abnormal Liver Chemistries. Am J Gastroenterol. 2017. doi:10.1038/ajg.2016.517](https://doi.org/10.1038/ajg.2016.517)

### I train regularly. Could hard exercise in the days before the test have raised my AST or ALT, and should we repeat after a few lighter days or check creatine kinase (CK)?

- **Asked when:** ALT or AST is flagged (asked once).
- **Rule:** `liver.panel.exercise`
- **Why:** After one hour of weightlifting, AST and ALT rose significantly in healthy men and stayed raised for at least 7 days. — [Pettersson J, Hindorf U, Persson P, et al. Muscular exercise can cause highly pathological liver function tests in healthy men. Br J Clin Pharmacol. 2008;65(2):253-259. doi:10.1111/j.1365-2125.2007.03001.x](https://doi.org/10.1111/j.1365-2125.2007.03001.x)
- **Why:** Lists strenuous exercise and muscle injury as non-liver causes of raised AST/ALT, with creatine kinase as the first check for a muscle source. — [Kwo PY, Cohen SM, Lim JK. ACG Clinical Guideline: Evaluation of Abnormal Liver Chemistries. Am J Gastroenterol. 2017. doi:10.1038/ajg.2016.517](https://doi.org/10.1038/ajg.2016.517)

### Should a FIB-4 score be calculated to check my risk of liver scarring, for example from fatty liver?

- **Asked when:** ALT or AST is flagged (asked once).
- **Rule:** `liver.panel.fib4`
- **Why:** Recommends a first risk assessment with the FIB-4 score for people with suspected fatty liver or metabolic risk factors; FIB-4 below 1.3 indicates low risk. — [Rinella ME, Neuschwander-Tetri BA, Siddiqui MS, et al. AASLD Practice Guidance on the clinical assessment and management of nonalcoholic fatty liver disease. Hepatology. 2023. doi:10.1097/HEP.0000000000000323](https://doi.org/10.1097/HEP.0000000000000323)

### My alkaline phosphatase was [your result]. Should a GGT test check whether it comes from the liver or from bone?

- **Asked when:** Alkaline phosphatase is high and no GGT is on record.
- **Rule:** `liver.alp.ggt`
- **Why:** Recommends confirming a raised alkaline phosphatase with GGT (or ALP fractionation) to show whether it comes from the liver. — [Kwo PY, Cohen SM, Lim JK. ACG Clinical Guideline: Evaluation of Abnormal Liver Chemistries. Am J Gastroenterol. 2017. doi:10.1038/ajg.2016.517](https://doi.org/10.1038/ajg.2016.517)

### My bilirubin was [your result]. Should it be split into direct and indirect bilirubin? If only indirect is mildly raised and my other liver tests are normal, could it be Gilbert syndrome?

- **Asked when:** Bilirubin is high.
- **Rule:** `liver.bilirubin.fractionate`
- **Why:** Recommends fractionating raised total bilirubin, and says mild unconjugated bilirubin with normal liver enzymes in a healthy person usually suggests Gilbert syndrome. — [Kwo PY, Cohen SM, Lim JK. ACG Clinical Guideline: Evaluation of Abnormal Liver Chemistries. Am J Gastroenterol. 2017. doi:10.1038/ajg.2016.517](https://doi.org/10.1038/ajg.2016.517)

## Blood count and iron

### I do endurance training. Could extra plasma volume from training ("sports anemia") explain part of my lower hemoglobin or hematocrit, and what would rule out a real anemia?

- **Asked when:** Hemoglobin or hematocrit is low (asked once).
- **Rule:** `cbc.panel.training`
- **Why:** Endurance-trained athletes often have a slightly lower hematocrit ("sports anemia") because training expands plasma volume, while their total red-cell mass is higher. — [Mairbäurl H. Red blood cells in sports: effects of exercise and training on oxygen supply by red blood cells. Front Physiol. 2013;4:332. doi:10.3389/fphys.2013.00332](https://doi.org/10.3389/fphys.2013.00332)

### Should iron studies, including ferritin, be checked?

- **Asked when:** Hemoglobin or hematocrit is low and no ferritin is on record.
- **Rule:** `cbc.panel.iron_studies`
- **Why:** Recommends defining iron deficiency by a ferritin below 45 ng/mL (rather than 15 ng/mL) in people with anemia. — [Ko CW, Siddique SM, Patel A, et al. AGA Clinical Practice Guidelines on the Gastrointestinal Evaluation of Iron Deficiency Anemia. Gastroenterology. 2020. doi:10.1053/j.gastro.2020.06.046](https://doi.org/10.1053/j.gastro.2020.06.046)

### My ferritin was [your result]. Does this suggest low iron stores, and should we look for a cause?

- **Asked when:** Ferritin is low or below 45 ng/mL.
- **Rule:** `iron.ferritin.low`
- **Why:** Recommends defining iron deficiency by a ferritin below 45 ng/mL (rather than 15 ng/mL) in people with anemia. — [Ko CW, Siddique SM, Patel A, et al. AGA Clinical Practice Guidelines on the Gastrointestinal Evaluation of Iron Deficiency Anemia. Gastroenterology. 2020. doi:10.1053/j.gastro.2020.06.046](https://doi.org/10.1053/j.gastro.2020.06.046)

## Electrolytes

### My potassium was [your result]. Could the blood draw itself (fist clenching, a tight tourniquet or a delayed sample) have raised it, and should it be repeated?

- **Asked when:** Potassium is high.
- **Rule:** `lytes.potassium.high`
- **Why:** Explains that blood-draw factors such as hemolysis, fist clenching, a prolonged tourniquet, delayed processing or very high platelet or white cell counts can falsely raise potassium. — [Acute Care Testing (Radiometer). Pseudohyperkalemia (review, citing Don BR et al., N Engl J Med 1990;322:1290-1292).](https://acutecaretesting.org/en/articles/pseudohyperkalemia)

### My sodium was [your result]. Could drinking more fluid than I lost around long training sessions have lowered it, and should it be rechecked?

- **Asked when:** Sodium is low.
- **Rule:** `lytes.sodium.low`
- **Why:** Defines exercise-associated hyponatremia as low sodium during or up to 24 hours after activity, mainly from drinking more fluid than is lost. — [Hew-Butler T, Rosner MH, Fowkes-Godek S, et al. Statement of the 3rd International Exercise-Associated Hyponatremia Consensus Development Conference, Carlsbad, California, 2015. Br J Sports Med. 2015;49(22):1432.](https://bjsm.bmj.com/content/49/22/1432)

## Thyroid

### My TSH was [your result]. Should it be repeated in 2–3 months with a free T4, and not during an illness, to see whether it persists?

- **Asked when:** TSH is high.
- **Rule:** `thyroid.tsh.high`
- **Why:** Advises re-testing a mildly raised TSH (4–10 mIU/L) with normal free T4 after 2–3 months, with thyroid antibodies, and delaying testing during an acute illness (citing NICE NG145). — [Royal Australian College of General Practitioners. Management of subclinical hypothyroidism (First Do No Harm), revised 2022, citing NICE NG145 (2019).](https://www.racgp.org.au/clinical-resources/clinical-guidelines/first-do-no-harm/gp-resources/management-of-subclinical-hypothyroidism)

## Vitamin D

### My vitamin D was [your result]. Does this result need follow-up or retesting for me, given that routine testing isn't advised for most healthy adults?

- **Asked when:** Vitamin D is flagged.
- **Rule:** `vitd.followup`
- **Why:** Suggests against routine vitamin D (25(OH)D) testing in healthy adults, and notes that levels giving specific health benefits have not been established in trials. — [Demay MB, Pittas AG, Bikle DD, et al. Vitamin D for the Prevention of Disease: An Endocrine Society Clinical Practice Guideline. J Clin Endocrinol Metab. 2024. doi:10.1210/clinem/dgae290](https://doi.org/10.1210/clinem/dgae290)

## Any flagged result

### Could something temporary explain my [test name] result of [your result], such as what I ate or drank, a medicine or supplement, or hard exercise before the test?

- **Asked when:** Any flagged result with no reviewed specific questions.
- **Rule:** `general.explain`
- **Why:** Lists foods and drinks, medicines or supplements, and hard exercise before a test among the things that can affect results. — [MedlinePlus, U.S. National Library of Medicine. How to Understand Your Lab Results.](https://medlineplus.gov/lab-tests/how-to-understand-your-lab-results/)

### Should this test be repeated to confirm the result, and if so when?

- **Asked when:** Any flagged result with no reviewed specific questions.
- **Rule:** `general.repeat`
- **Why:** Says a result that may be inaccurate or is uncertain is often tested again. — [MedlinePlus, U.S. National Library of Medicine. How to Understand Your Lab Results.](https://medlineplus.gov/lab-tests/how-to-understand-your-lab-results/)
- **Why:** Reference intervals cover the central 95% of healthy people, so about 5% of healthy results fall outside them and are flagged. — [Ozarda Y. Reference intervals: current status, recent developments and future considerations. Biochem Med (Zagreb). 2016;26(1):5-11. doi:10.11613/BM.2016.001](https://doi.org/10.11613/BM.2016.001)

### My previous [test name] was [your result] on [earlier date]. Is the change meaningful, and were both tests from the same lab?

- **Asked when:** Any flagged result with no reviewed specific questions and an earlier result on record.
- **Rule:** `general.trend`
- **Why:** Advises using the same lab when looking at trends, because results from different labs can't be directly compared. — [MedlinePlus, U.S. National Library of Medicine. How to Understand Your Lab Results.](https://medlineplus.gov/lab-tests/how-to-understand-your-lab-results/)

## Before a blood test

Shown once you set a blood test date. The fasting item appears only if you say you were asked to fast.

- **Keep training easy for the 3 days before, and skip heavy or new strength work in the week before.** Hard exercise before a test can affect results; one hour of weightlifting kept AST and ALT raised for at least 7 days in healthy men. — [Pettersson J, Hindorf U, Persson P, et al. Muscular exercise can cause highly pathological liver function tests in healthy men. Br J Clin Pharmacol. 2008;65(2):253-259. doi:10.1111/j.1365-2125.2007.03001.x](https://doi.org/10.1111/j.1365-2125.2007.03001.x); [MedlinePlus, U.S. National Library of Medicine. How to Understand Your Lab Results.](https://medlineplus.gov/lab-tests/how-to-understand-your-lab-results/)
- **You were asked to fast: nothing but water for at least 8 hours before the draw.** Fasting glucose thresholds apply after at least 8 hours without calories. — [American Diabetes Association Professional Practice Committee. 2. Diagnosis and Classification of Diabetes: Standards of Care in Diabetes—2026. Diabetes Care. 2026;49(Suppl 1):S27. doi:10.2337/dc26-S002](https://doi.org/10.2337/dc26-s002)
- **Ask your doctor or lab whether any medicine or supplement should be paused before the test.** Medicines and supplements are among the things that can affect results. — [MedlinePlus, U.S. National Library of Medicine. How to Understand Your Lab Results.](https://medlineplus.gov/lab-tests/how-to-understand-your-lab-results/)
- **During the draw, keep your hand relaxed: don't pump or clench your fist.** Fist clenching, a long tourniquet or a delayed sample can falsely raise potassium. — [Acute Care Testing (Radiometer). Pseudohyperkalemia (review, citing Don BR et al., N Engl J Med 1990;322:1290-1292).](https://acutecaretesting.org/en/articles/pseudohyperkalemia)
- **If you can, use the same lab as last time so your trends compare fairly.** Results from different labs can't be directly compared when looking at trends. — [MedlinePlus, U.S. National Library of Medicine. How to Understand Your Lab Results.](https://medlineplus.gov/lab-tests/how-to-understand-your-lab-results/)

## Scores POM calculates

Shown with the formula, every input and the source; context for your clinician, not a diagnosis, and not clinician-reviewed.

### FIB-4 score

- **Shown when:** A liver result (AST or ALT) is flagged and AST, ALT and platelets come from the same blood draw.
- **Formula:** FIB-4 = (age × AST) ÷ (platelets × √ALT)
- **Reading:** Below 1.3 is described as low risk of advanced fibrosis (AASLD 2023).
- **Source:** Defines FIB-4 as (age × AST) / (platelets × √ALT), with age in years, AST and ALT in U/L and platelets in 10⁹/L. — [Sterling RK, Lissen E, Clumeck N, et al. Development of a simple noninvasive index to predict significant fibrosis in patients with HIV/HCV coinfection. Hepatology. 2006;43(6):1317-1325. doi:10.1002/hep.21178](https://doi.org/10.1002/hep.21178)
- **Source:** Recommends a first risk assessment with FIB-4; FIB-4 below 1.3 indicates low risk of advanced fibrosis. — [Rinella ME, Neuschwander-Tetri BA, Siddiqui MS, et al. AASLD Practice Guidance on the clinical assessment and management of nonalcoholic fatty liver disease. Hepatology. 2023. doi:10.1097/HEP.0000000000000323](https://doi.org/10.1097/HEP.0000000000000323)

### 10-year cardiovascular risk (PREVENT)

- **Shown when:** A cholesterol result is flagged and age 30–79, sex, total cholesterol, HDL, eGFR, systolic blood pressure (Apple Health or entered) and the yes/no questions are all known.
- **Formula:** PREVENT base 10-year equations for total CVD and ASCVD (Khan 2024), coefficients from preventr
- **Reading:** Shown against the 2026 ACC/AHA PREVENT-ASCVD categories: <3%, 3% to <5% borderline, 5% to <10% intermediate, ≥10%.
- **Source:** PREVENT estimates 10-year cardiovascular risk for adults aged 30–79 from age, sex, cholesterol, HDL, blood pressure, diabetes, smoking, kidney function and blood pressure and statin treatment. — [Khan SS, Matsushita K, Sang Y, et al. Development and validation of the American Heart Association's PREVENT equations. Circulation. 2024;149:430-449. doi:10.1161/CIRCULATIONAHA.123.067626](https://doi.org/10.1161/CIRCULATIONAHA.123.067626)
- **Source:** Uses 10-year PREVENT-ASCVD risk categories: borderline 3% to <5%, intermediate 5% to <10%. — [Blumenthal RS, Morris PB, Gaudino M, et al. 2026 ACC/AHA Guideline on the Management of Dyslipidemia. Circulation. 2026. doi:10.1161/CIR.0000000000001423](https://doi.org/10.1161/CIR.0000000000001423)
- **Source:** Open-source implementation POM's coefficients and variable transformations were taken from and tested against. — [Mayer MG. preventr: An implementation of the PREVENT and Pooled Cohort Equations (R package, CRAN).](https://cran.r-project.org/web/packages/preventr/)

## All sources

| Source | Type | Last reviewed |
| --- | --- | --- |
| [Blumenthal RS, Morris PB, Gaudino M, et al. 2026 ACC/AHA/AACVPR/ABC/ACPM/ADA/AGS/APhA/ASPC/NLA/PCNA Guideline on the Management of Dyslipidemia. Circulation. 2026. doi:10.1161/CIR.0000000000001423](https://doi.org/10.1161/CIR.0000000000001423) | guideline | 2026-10-20 |
| [Kronenberg F, Mora S, Stroes ESG, et al. Lipoprotein(a) in atherosclerotic cardiovascular disease and aortic stenosis: a European Atherosclerosis Society consensus statement. Eur Heart J. 2022. doi:10.1093/eurheartj/ehac361](https://doi.org/10.1093/eurheartj/ehac361) | consensus | 2026-10-20 |
| [Sniderman AD, Thanassoulis G, Glavinovic T, et al. Apolipoprotein B particles and cardiovascular disease: a narrative review. JAMA Cardiol. 2019;4(12):1287-1295. doi:10.1001/jamacardio.2019.3780](https://doi.org/10.1001/jamacardio.2019.3780) | study | 2026-10-20 |
| [Budoff MJ, Young R, Burke G, et al. Ten-year association of coronary artery calcium with atherosclerotic cardiovascular disease (ASCVD) events: the Multi-Ethnic Study of Atherosclerosis (MESA). Eur Heart J. 2018;39(25):2401-2408. doi:10.1093/eurheartj/ehy217](https://doi.org/10.1093/eurheartj/ehy217) | study | 2026-10-20 |
| [Khan SS, Matsushita K, Sang Y, et al. Development and validation of the American Heart Association's PREVENT equations. Circulation. 2024;149:430-449. doi:10.1161/CIRCULATIONAHA.123.067626](https://doi.org/10.1161/CIRCULATIONAHA.123.067626) | study | 2026-10-20 |
| [MedlinePlus, U.S. National Library of Medicine. How to Understand Your Lab Results.](https://medlineplus.gov/lab-tests/how-to-understand-your-lab-results/) | reference | 2026-10-20 |
| [Ozarda Y. Reference intervals: current status, recent developments and future considerations. Biochem Med (Zagreb). 2016;26(1):5-11. doi:10.11613/BM.2016.001](https://doi.org/10.11613/BM.2016.001) | study | 2026-10-20 |
| [American Diabetes Association Professional Practice Committee. 2. Diagnosis and Classification of Diabetes: Standards of Care in Diabetes—2026. Diabetes Care. 2026;49(Suppl 1):S27. doi:10.2337/dc26-S002](https://doi.org/10.2337/dc26-s002) | guideline | 2026-10-20 |
| [US Preventive Services Task Force. Screening for Prediabetes and Type 2 Diabetes: US Preventive Services Task Force Recommendation Statement. JAMA. 2021. doi:10.1001/jama.2021.12531](https://www.uspreventiveservicestaskforce.org/uspstf/recommendation/screening-for-prediabetes-and-type-2-diabetes) | guideline | 2026-10-20 |
| [Diabetes Prevention Program Research Group. Reduction in the incidence of type 2 diabetes with lifestyle intervention or metformin. N Engl J Med. 2002;346(6):393-403. doi:10.1056/NEJMoa012512](https://doi.org/10.1056/NEJMoa012512) | study | 2026-10-20 |
| [Kidney Disease: Improving Global Outcomes (KDIGO) CKD Work Group. KDIGO 2024 Clinical Practice Guideline for the Evaluation and Management of Chronic Kidney Disease. Kidney Int. 2024;105(4S):S117-S314.](https://kdigo.org/wp-content/uploads/2026/05/KDIGO-2024-CKD-Guideline-Summary-Recommendations-and-Practice-Points.pdf) | guideline | 2026-10-20 |
| [Kwo PY, Cohen SM, Lim JK. ACG Clinical Guideline: Evaluation of Abnormal Liver Chemistries. Am J Gastroenterol. 2017. doi:10.1038/ajg.2016.517](https://doi.org/10.1038/ajg.2016.517) | guideline | 2026-10-20 |
| [Pettersson J, Hindorf U, Persson P, et al. Muscular exercise can cause highly pathological liver function tests in healthy men. Br J Clin Pharmacol. 2008;65(2):253-259. doi:10.1111/j.1365-2125.2007.03001.x](https://doi.org/10.1111/j.1365-2125.2007.03001.x) | study | 2026-10-20 |
| [Rinella ME, Neuschwander-Tetri BA, Siddiqui MS, et al. AASLD Practice Guidance on the clinical assessment and management of nonalcoholic fatty liver disease. Hepatology. 2023. doi:10.1097/HEP.0000000000000323](https://doi.org/10.1097/HEP.0000000000000323) | guideline | 2026-10-20 |
| [Mairbäurl H. Red blood cells in sports: effects of exercise and training on oxygen supply by red blood cells. Front Physiol. 2013;4:332. doi:10.3389/fphys.2013.00332](https://doi.org/10.3389/fphys.2013.00332) | study | 2026-10-20 |
| [Ko CW, Siddique SM, Patel A, et al. AGA Clinical Practice Guidelines on the Gastrointestinal Evaluation of Iron Deficiency Anemia. Gastroenterology. 2020. doi:10.1053/j.gastro.2020.06.046](https://doi.org/10.1053/j.gastro.2020.06.046) | guideline | 2026-10-20 |
| [Hew-Butler T, Rosner MH, Fowkes-Godek S, et al. Statement of the 3rd International Exercise-Associated Hyponatremia Consensus Development Conference, Carlsbad, California, 2015. Br J Sports Med. 2015;49(22):1432.](https://bjsm.bmj.com/content/49/22/1432) | consensus | 2026-10-20 |
| [Acute Care Testing (Radiometer). Pseudohyperkalemia (review, citing Don BR et al., N Engl J Med 1990;322:1290-1292).](https://acutecaretesting.org/en/articles/pseudohyperkalemia) | reference | 2026-10-20 |
| [Royal Australian College of General Practitioners. Management of subclinical hypothyroidism (First Do No Harm), revised 2022, citing NICE NG145 (2019).](https://www.racgp.org.au/clinical-resources/clinical-guidelines/first-do-no-harm/gp-resources/management-of-subclinical-hypothyroidism) | guideline | 2026-10-20 |
| [Demay MB, Pittas AG, Bikle DD, et al. Vitamin D for the Prevention of Disease: An Endocrine Society Clinical Practice Guideline. J Clin Endocrinol Metab. 2024. doi:10.1210/clinem/dgae290](https://doi.org/10.1210/clinem/dgae290) | guideline | 2026-10-20 |
