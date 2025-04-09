# Personalized-Mentor-Recommendation-System
Personalized Mentor Recommendation System recommends top CLAT toppers (mentors) to aspirants based on their profiles.

I have used content-based recommendation approach - cosine similarity, which measures how closely aligned an aspirant’s preferences are with each mentor’s profile.
How It Works:
The features for both aspirants and mentors are vectorized using techniques like:

1. MultiLabelBinarizer for multi-choice features (subjects and colleges)

2. One-Hot Encoding for categorical features (learning style)

3. Once encoded, each profile becomes a feature vector.

I computed the cosine similarity between an aspirant and all available mentors.

The top 3 mentors with the highest similarity scores are recommended to the aspirant.

This approach ensures that recommendations are personalized based on profile similarity.
