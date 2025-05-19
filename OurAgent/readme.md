### An Automated Ultrasound Diagnostic Agent

In this paper, we have constructed an intelligent agent named **An Automated Ultrasound Diagnostic Agent** designed for assisting in ultrasound diagnostics.

#### Introduction

**An Automated Ultrasound Diagnostic Agent** is an innovative intelligent agent designed to assist ultrasound imaging diagnostic experts in clinical decision-making. This agent leverages an advanced machine learning model based on **DeepSeek-R1-7B** to provide possible condition diagnoses and professional diagnostic recommendations based on patient complaints, physical examination results, and additional information.

#### Features

- **Automated Diagnostic Suggestions:** Quickly generate preliminary diagnoses based on input clinical information.
- **Diagnostic Justification:** Provide detailed reasoning to support preliminary diagnoses, aiding doctors in understanding the basis for the diagnosis.
- **Recommended Follow-Up Examinations:** Suggest necessary follow-up examinations and monitoring based on preliminary diagnoses.


#### Usage

##### Prompts


> You are a senior ultrasound imaging diagnostic expert. Based on the information below, determine the patient's possible condition and provide diagnostic recommendations.
Model Classification Result: <Model_Result>
Chief Complaint:<Chief_Complaint>
Physical Examination:<Physical_Exam>
Additional Information:<Additional_Info>
>
> Please reason according to international diagnostic guidelines and generate a medically standardized recommendation using professional terminology. The output format should be:
> 
> 1.Preliminary Diagnosis:
2.Justification:
3.Recommended Follow-Up Examinations:

### Test Cases

We have tested **two real clinical cases**, and the inputs and outputs are recorded in the [case.docx](./case.docx) file. These cases demonstrate the **application and accuracy of the intelligent agent in actual clinical settings.**

###  Evaluate criterion


Our intelligent agent's performance is **evaluated using a weighted scoring system:**

$$
\text{Final Score} = 0.2 \times S_{\text{amateur}} + 0.6 \times S_{\text{expert}} + 0.2 \times 5 \times M
$$

- $ S_{\text{amateur}} $ : Average score from non-experts 
- $  S_{\text{expert}} $: Average score from experts 
- $ M $: METEOR score for semantic similarity


### Extending Usage

You can use our intelligent agent to test **additional cases** by following the prompts format provided. This can help you **assess the performance** of the agent across a broader range of clinical scenarios.

### Contact

For any questions or further information, please contact the corresponding author of this project.
