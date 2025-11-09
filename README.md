---

# 🧠 Review Analyzer – AI-Powered Customer Insights Dashboard

An end-to-end AI web application that analyzes customer reviews and visualizes actionable insights through an interactive dashboard.
Built with **Next.js**, **React**, and **Scoutos AI**, this system combines advanced NLP workflows and intuitive data visualization to help businesses understand customer sentiment, detect issues, and improve products.

---

## 🚀 Overview

The **Review Analyzer** consists of two integrated parts:

1. **Frontend Dashboard:**
   A sleek, interactive web application where users can upload reviews and explore insights through charts and metrics.

2. **Scout AI Workflow:**
   A large language model (LLM)-powered backend workflow built in [Scout](https://scoutos.com/) that performs in-depth text analysis and returns structured results in JSON format.

Together, they form a full-stack AI solution for **sentiment analysis**, **aspect extraction**, **trend detection**, and **recommendation generation**.

---

## 🎯 Key Features

### 🧩 Sentiment Analysis

* Automatically classifies reviews as positive, neutral, or negative
* Displays overall sentiment ratios with visual indicators
* Tracks trends over time with interactive charts

### 💬 Aspect-Based Insights

* Breaks feedback into categories such as **product quality**, **usability**, **pricing**, **delivery**, and **customer service**
* Visualizes aspect-specific sentiment balance
* Highlights strengths and weaknesses across business areas

### ⚠️ Recurring Issues & Feature Requests

* Detects common customer complaints and pain points
* Extracts customer feature requests with priority levels
* Helps teams focus on the most impactful improvements

### 🧠 Actionable Recommendations

* Generates data-driven improvement ideas directly from customer feedback
* Prioritizes recommendations by frequency and sentiment weight

---

## 🧩 System Architecture

### 🔹 Frontend

* **Next.js 14** – React framework with server-side rendering
* **React 19** – Modular and dynamic UI components
* **Tailwind CSS** – Responsive, utility-first design
* **Shadcn/UI** – Accessible and themeable UI components
* **Framer Motion** – Smooth animations and transitions
* **Chart.js / React-chartjs-2** – Data visualization and analytics
* **React Circular Progressbar** – Circular metrics indicators

### 🔹 Backend & AI Workflow

* **Scoutos AI Workflow** handles all text analysis using LLM reasoning blocks:

  1. **Input Block:** Collects raw customer reviews
  2. **LLM Analysis Block:** Performs sentiment and aspect-based analysis
  3. **JSON Formatter Block:** Structures results for the frontend dashboard
* Results are securely fetched via API and rendered in real time

---

## 📊 Data Flow

1. User uploads a file containing customer reviews
2. `/api/upload` endpoint sends data to the Scout AI workflow
3. Workflow analyzes the text using LLM reasoning
4. JSON output is returned and stored server-side
5. Dashboard visualizes structured results through charts and cards
6. Users can filter, explore, and export insights

---

## 🔒 Security

* API keys and credentials stored in environment variables
* Secure server-side proxy for AI requests
* Input validation on both client and server
* No sensitive data exposed to the frontend

---

## 🌙 Theme Support

* System theme detection
* Manual dark/light mode toggle
* Persistent user preference
* Accessible color contrast for both modes

---

## 🧠 Example Input and Output (from AI Workflow)

```"I love the product quality, but the delivery was delayed. Customer service was helpful, but pricing feels a bit high compared to competitors."```

```json
{
  "sentimentAnalysis": {
    "positive": 60,
    "neutral": 10,
    "negative": 30
  },
  "aspectAnalysis": {
    "productQuality": "positive",
    "pricing": "negative",
    "delivery": "negative"
  },
  "recurringIssues": ["late delivery", "high pricing"],
  "recommendations": [
    "Optimize shipping process",
    "Reconsider pricing strategy"
  ]
}
```

---

## 🎓 Academic Project

Developed as part of a **diploma thesis** focusing on:

* AI workflow automation and NLP integration
* Advanced web development with Next.js and React
* Data visualization and user experience design
* Real-world application of LLMs for business analytics

---

## 🤝 Contributing

Contributions are welcome!
Feel free to open issues or submit pull requests to improve functionality or design.

---

## 📄 License

MIT License — free for educational and personal use.

---

**Built with ❤️ using Next.js, React, Tailwind, and Scoutos AI**

---
