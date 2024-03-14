This project aims to develop a music recommendation system using the AudioSet dataset provided by Google. AudioSet is a large-scale dataset that consists of manually annotated audio events from YouTube videos, covering a wide range of categories including music.

The steps to run the project are as follows:

Download the Dataset: Access the AudioSet dataset from the provided link(https://research.google.com/audioset/download.html). This dataset contains YouTube videos that have been encoded using the MAX-Audio-Embedding-Generator.

Extract Music Audio: Ensure that only music audio is extracted from the dataset. Since AudioSet contains various types of audio events, it's crucial to filter out non-music audio to focus on music recommendations.

Cut Audio Clips: Once the music audio is extracted, cut each audio clip to be 10 seconds in duration. This standardizes the length of audio samples, making them suitable for comparison and recommendation purposes.

Store in JSON Format: Store the preprocessed audio samples in a list of JSON objects. Each JSON object represents an audio sample with metadata such as the audio features and labels.

Nearest Neighbor Algorithm: Utilize the ANNOY (Approximate Nearest Neighbors Oh Yeah) algorithm to build a nearest neighbor search index for the audio samples. This algorithm efficiently finds the closest neighbors to a given input audio sample based on their feature embeddings.

Recommendation Generation: Implementing a system that takes an input audio sample and utilizes the ANNOY index to retrieve a list of recommended music tracks from the dataset. These recommendations are based on the similarity of audio features between the input sample and the samples in the dataset.


By following these steps and running the provided notebook , users can experience the functionality of the music recommendation system and explore personalized music recommendations based on their input audio samples.
