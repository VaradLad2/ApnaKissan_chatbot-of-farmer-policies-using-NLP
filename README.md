
# Apna Kissan 🌾🤖

**Apna Kissan** is an AI-powered chatbot designed to assist farmers with information about Indian government farming schemes. It helps farmers access details about schemes, eligibility, benefits, and more, enabling them to make informed decisions for their agricultural needs.

---

## 🚀 Features

- **Scheme Matching:** Matches user queries to relevant Indian farming schemes using TF-IDF and cosine similarity.
- **Intent Recognition:** Identifies user intent (e.g., financial support, eligibility, small talk) using zero-shot classification.
- **Farming Advice:** Offers tips and recommendations for common farming challenges.
- **Interactive Chat:** Handles queries in real-time with a user-friendly conversational interface.
- **Easy Deployment:** Hosted via Flask API, with ngrok support for local testing and web access.

---

## 🛠️ Tech Stack

- **Programming Language:** Python
- **Libraries Used:**
  - [SpaCy](https://spacy.io) for NLP preprocessing
  - [Transformers](https://huggingface.co/transformers/) for intent classification
  - [Scikit-learn](https://scikit-learn.org/) for vectorization and similarity matching
  - [TheFuzz](https://github.com/seatgeek/thefuzz) for fuzzy matching
  - [Flask](https://flask.palletsprojects.com/) for API hosting
- **Deployment Tools:** ngrok, joblib

---

## 🧰 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/VaradLad2/ApnaKissan_chatbot-of-farmer-policies-using-NLP.git
   cd ApnaKissan_chatbot-of-farmer-policies-using-NLP
   ```

2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Place the dataset (`indian_farmer_schemes_large.xlsx`) in the root directory.

4. Run the Flask server:
   ```bash
   python app.py
   ```

5. Access the chatbot API:
   - Locally at `http://127.0.0.1:5000`
   - Or via ngrok (if configured).

---

## 🧑‍💻 How It Works

1. **Preprocessing:**
   - The dataset is cleaned and normalized for efficient matching.

2. **Query Matching:**
   - User input is matched to the closest farming scheme using TF-IDF cosine similarity and fuzzy matching.

3. **Intent Detection:**
   - The chatbot classifies user queries into intents like benefits, eligibility, application process, etc.

4. **Response Generation:**
   - Relevant scheme details or farming advice is provided based on the identified intent.

---

## 📄 API Endpoints

- **POST /chat**
  - Request: `{"message": "Your query here"}`
  - Response: `{"response": "Chatbot's reply"}`

---

## 🗂️ Project Structure

```
ApnaKissan_chatbot-of-farmer-policies-using-NLP/
├── app.py                  # Flask application
├── dataset/
│   └── indian_farmer_schemes_large.xlsx  # Farming schemes dataset
├── models/
│   ├── tfidf_vectorizer.pkl # Saved vectorizer model
│   ├── scheme_vectors.pkl   # Preprocessed scheme vectors
│   └── farmer_chatbot.pkl   # Chatbot model
├── static/
│   └── ...                  # Static assets (if any)
├── templates/
│   └── ...                  # HTML templates (if needed)
├── requirements.txt         # Dependencies
└── README.md                # Project documentation
```

---

## 🤝 Contributing

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add your feature"
   ```
4. Push to the branch:
   ```bash
   git push origin feature/your-feature-name
   ```
5. Open a pull request.

---

## 📧 Contact

For any questions or feedback, feel free to reach out at **varadlad2@gmail.com**.

---

## 📜 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

### 🌟 Show Your Support

If you find this project helpful, give it a ⭐ on GitHub and share it with others!
```

Make sure to replace any placeholder paths or details with the actual ones relevant to your repository. Let me know if you'd like further refinements!
