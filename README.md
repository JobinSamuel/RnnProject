# 🎬 IMDB Movie Review Sentiment Analysis (SimpleRNN + Streamlit)

This project is a complete **end-to-end Deep Learning NLP application** that classifies IMDB movie reviews as:

✅ **Positive**
❌ **Negative**

It uses a **SimpleRNN model trained on the IMDB dataset (TensorFlow/Keras)** and is deployed as an interactive **Streamlit web app** where users can enter a review and instantly get sentiment predictions.

---

##  What This Project Does

* Loads a pre-trained **SimpleRNN sentiment classification model**
* Converts user text input into tokenized format using IMDB word index
* Pads reviews to a fixed length for consistent model input
* Predicts sentiment score in real-time
* Displays:

  * Sentiment label (**Positive / Negative**)
  * Prediction confidence score

This is a practical example of taking an NLP deep learning model and deploying it into a working web app.


---

## Core Implementation (main.py)

The Streamlit app:

* Loads the IMDB word index
* Preprocesses text input
* Runs model inference
* Displays prediction results in UI 


---

## ▶️ Run the App Locally

### 1) Install dependencies

```bash
pip install streamlit tensorflow numpy
```

### 2) Start Streamlit

```bash
streamlit run main.py
```

---

## Example Output

* **Input:** “This movie was amazing and had a great story”
* **Prediction:** Positive
* **Score:** 0.9+

---

## Notes

* The model expects input padded to **max length 500** for consistency 
* Sentiment decision threshold:

  * `> 0.5` → **Positive**
  * `<= 0.5` → **Negative** 

