# TikTok's Claims Classification Project  

TikTok users have the ability to report videos and comments that contain user claims. These reports identify content that needs to be reviewed by moderators. This process generates a large number of user reports that are difficult to address quickly.  

This project aims to develop a predictive model that can determine whether a video contains a claim or offers an opinion. With a successful prediction model, TikTok can reduce the backlog of user reports and prioritize them more efficiently.  

---

## Project Overview  

The project is divided into five main components, each addressing a specific aspect of the data analysis and modeling process:

1. **Inspection and Analysis:**  
   Initial exploration of the dataset to understand its structure, handle missing values, and inspect data distributions. This step provides a foundation for subsequent analysis.  

2. **EDA and DataViz:**  
   Exploratory Data Analysis (EDA) and visualization of key variables to uncover patterns, relationships, and trends in the dataset, such as the characteristics of reported videos and comments, the distribution of claims vs. opinions, and user reporting behavior.

3. **Stats and Hypothesis Testing:**  
   Performing statistical analysis and hypothesis testing to determine significant factors influencing whether content is labeled as a claim or an opinion. These insights can validate model assumptions and guide feature engineering.

4. **Logistic Regression:**  
   Building a logistic regression model to predict verified status, offering insights into how video characteristics relate to claims and verified users. This step provides a simpler, interpretable baseline model.  

5. **Random Forest Model:**  
   Developing a Random Forest classifier to predict whether a TikTok video presents a "claim" or an "opinion." This model aims to improve prediction accuracy and handle complex relationships in the data.  

---

## Machine Learning  

- **Purpose:**  
   To predict whether TikTok content contains a claim or an opinion, enabling efficient moderation and prioritization of flagged reports.  

- **Approach:**  
   - Logistic Regression serves as a baseline model for classification and interpretability.  
   - Random Forest and XGBoost are implemented for more robust and accurate classification.  

---

## Technologies Used  

- **Programming Language:** Python  
- **Libraries:**  
  - Data Manipulation: Pandas, NumPy  
  - Visualization: Matplotlib, Seaborn  
  - Data Preprocessing: Scikit-learn  
  - Machine Learning: Scikit-learn, XGBoost  
- **Development Environment:** Jupyter Notebooks  

---

## Dataset Description  

This project uses a synthetic dataset called **tiktok_dataset.csv**, created in partnership with TikTok. It contains 19,383 rows, with each row representing a different published TikTok video in which a claim or opinion has been made. The dataset includes 12 columns, each representing different attributes related to the video and its status.

Here are the details of the columns in the dataset:

| Column Name          | Type  | Description                                                                                           |
|----------------------|-------|-------------------------------------------------------------------------------------------------------|
| **#**                | int   | TikTok assigned number for the video with a claim or opinion.                                          |
| **claim_status**     | obj   | Whether the published video has been identified as an “opinion” or a “claim.” A “claim” refers to unsourced or unverified information. An “opinion” refers to a personal belief or thought. |
| **video_id**         | int   | Random identifying number assigned to the video upon publication on TikTok.                            |
| **video_duration_sec**| int   | Duration of the published video, measured in seconds.                                                 |
| **video_transcription_text** | obj | Transcribed text of the words spoken in the published video.                                         |
| **verified_status**  | obj   | Indicates the verification status of the TikTok user who published the video. Can be "verified" or "not verified". |
| **author_ban_status**| obj   | Indicates the status of the TikTok user in terms of their permissions: “active,” “under scrutiny,” or “banned.” |
| **video_view_count** | float | The total number of times the published video has been viewed.                                        |
| **video_like_count** | float | The total number of times the published video has been liked by other users.                          |
| **video_share_count**| float | The total number of times the published video has been shared by other users.                         |
| **video_download_count** | float | The total number of times the published video has been downloaded by other users.                     |
| **video_comment_count** | float | The total number of comments on the published video.                                                  |

---

## Usage  

To run the analysis and models, follow these steps:  

1. Open the Jupyter Notebooks in the project folder.  
2. Execute the notebooks in the following order:  
   - Inspection and Analysis  
   - EDA and DataViz  
   - Stats and Hypothesis Testing  
   - Logistic Regression  
   - Random Forest Model  

---

## License  

This project is licensed under the MIT License. See the LICENSE file for more details.  

---

## Acknowledgments  

- Google, Kaggle and TikTok for providing the project concept and dataset.  
- The Python and data science community for valuable tools and resources.  
