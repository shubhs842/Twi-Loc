## Twi-Loc: Location Based Analysis Using Machine Learning

Twi-Loc is a machine learning project aimed at predicting the geographical location of Twitter users based on their tweets. By leveraging advanced Natural Language Processing (NLP) and deep learning techniques, Twi-Loc provides insights into user behaviour and trends, offering applications ranging from targeted advertising to emergency response.

## Table of Contents
- Introduction
- Features
- Installation
- Usage
- Methodology
- Results
- Contributors
- License

## Introduction
In the age of social media, platforms like Twitter generate vast amounts of data that provide valuable insights into human behavior. One crucial application is geolocation prediction, which identifies a user's location based on their social media activity. This project addresses the challenges associated with predicting user locations using the sparse, noisy, and informal nature of Twitter data.

## Features
- Predicts the geolocation of Twitter users with high accuracy using machine learning.
- Integrates textual and metadata features for comprehensive analysis.
- Utilizes Convolutional Neural Networks (CNNs) to capture complex patterns in tweets.
- Supports multiple regions with varying prediction accuracies for North America, Europe, and Asia.

## Installation
1.  Clone the repository
    git clone https://github.com/yourusername/twi-loc.git
    cd twi-loc

2.	Install the required dependencies:
    pip install -r requirements.txt

3.	Obtain Twitter API credentials and set them up in a .env file:
    TWITTER_API_KEY=your_api_key
    TWITTER_API_SECRET=your_api_secret
    ACCESS_TOKEN=your_access_token
    ACCESS_TOKEN_SECRET=your_access_token_secret

## Usage
1.	Preprocess the data:
    python preprocess.py --input data/raw_tweets.csv --output data/processed_tweets.csv

2.	Train the model:
    python train.py --data data/processed_tweets.csv --model output/cnn_model.h5

3.	Make predictions:
    python predict.py --model output/cnn_model.h5 --input new_tweets.csv --output predictions.csv

## Methodology
1.	Data Collection: Tweets are gathered using the Twitter API, focusing on tweets with location information.
2.	Data Preprocessing: Text cleaning, tokenization, and vectorization using techniques like TF-IDF.
3.	Feature Extraction: CNN architecture processes textual data to extract spatial hierarchies.
4.	Model Training: A CNN is trained with 70% of the data, validated with 15%, and tested on the remaining 15%.
5.	Evaluation: The model's performance is measured using metrics like accuracy, precision, recall, and F1-score.
   
## Results
The model achieved the following metrics:
•	Overall Accuracy: 85%
•	Precision: 82%
•	Recall: 79%
•	F1-Score: 80.5%

## Regional Performance
•	North America: Accuracy = 88%, F1-Score = 84.5%
•	Europe: Accuracy = 82%, F1-Score = 79%
•	Asia: Accuracy = 84%, F1-Score = 82%

## Contributors
•	Akshaya Maujey
•	Sakshi Raghorte
•	Shubham Mohod
•	Vedant Karande
•	Tanmay Kapale

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## www.ijcrt.org  © 2024 IJCRT | Volume 12, Issue 4 April 2024 | ISSN: 2320-2882 
   https://drive.google.com/file/d/17NVYmZ_-soTJIYVjW1063wZ8cLwPgdAg/view?usp=drive_link
                   
## Images 

![image](https://github.com/user-attachments/assets/214440bd-d619-420d-a69f-f9ad6830707c)

![image](https://github.com/user-attachments/assets/51b52971-a4e4-4fd7-a81c-fbbfe656d763)

![image](https://github.com/user-attachments/assets/709a745c-6051-4b73-8f83-fa5572813894)

![image](https://github.com/user-attachments/assets/a403e741-7b93-40a0-90e7-f6c41f8fc90b)

![image](https://github.com/user-attachments/assets/6a0a1d74-8e75-43cc-b69d-e5cd006bb9a5)

![image](https://github.com/user-attachments/assets/e66aacee-4397-42fb-b976-ee5e04381e88)








