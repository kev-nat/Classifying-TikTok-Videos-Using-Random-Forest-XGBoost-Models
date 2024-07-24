# Classifying TikTok Videos Using Random Forest & XGBoost Models

### **Overview**
<p align="justify"> The objective of this project was to develop XGBoost and random forest models to detect claims and opinions. The final random forest model achieved an accuracy of 99%. According to this model, the most significant factors in identifying whether a TikTok video contains a "claim" or an "opinion" were the video_view_count, video_like_count, video_share_count, and video_download_count. </p>

<p align="justify"> The goal of this model is to reduce misinformation in TikTok videos. By implementing an effective prediction model, TikTok can decrease the backlog of user reports and prioritize them more effectively. </p>

### **Business Understanding**
<p align="justify"> TikTok users can report videos they believe breach the platform's terms of service. Given the millions of videos created and watched daily, numerous videos are reported—far too many for individual review by human moderators. Analysis shows that videos violating terms of service are more likely to present a claim rather than an opinion. Hence, distinguishing between claim and opinion videos is valuable. Videos identified as opinions will be less likely to be reviewed by human moderators. In contrast, videos identified as claims will undergo further sorting to determine review priority. For example, claim videos might be ranked by the number of reports, with the top percentage reviewed by humans daily. </p>

### **Data Understanding**
<p align="justify"> The dataset comprised around 19,382 records and 12 features. Each entry corresponds to a unique TikTok video that either presents a claim or an opinion, along with its associated metadata. The features included details such as video duration, transcription, view count, like count, and verification status. The bar chart below illustrates the relationship between claim status and verification status. </p>

![image](https://github.com/user-attachments/assets/2062e1b1-fb36-4d81-96c8-c6a7b0a41051)

<p align="justify"> Approximately 50.3% of the dataset consists of claims, while 49.7% consists of opinions, indicating a balanced outcome variable. Additionally, a feature was created to depict the distribution of video transcription text length for both claims and opinions. </p>

![image](https://github.com/user-attachments/assets/45bc39cf-02a2-4177-961b-7fb5ba2a4909)

### **Modeling and Evaluation**
<p align="justify"> A random forest model with 200 decision trees was used to identify feature importance. The plot below indicates that trip duration, distance, and fare cost were the top 3 factors in determining generous tippers from non-generous ones. he overall model performed with 99% accuracy and 99% precision. </p>

![image](https://github.com/user-attachments/assets/e2812717-5334-4007-91f1-dc7c95bf66d5)

### **Conclusion**
<p align="justify"> This model can aid TikTok human moderators by reducing the backlog of user reports and improving prioritization efficiency. By presenting human moderators with videos most likely to violate TikTok's terms of service, this machine learning model significantly enhances their efforts. </p>
