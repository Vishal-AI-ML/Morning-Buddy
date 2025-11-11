# ☀️ Morning Buddy - AI-Powered Personal Assistant
An intelligent morning companion that helps you start your day right with personalized weather updates, curated news, and smart day planning using Google's Gemini AI.

## 🌟 Features

### 1. **Smart Weather Assistant**
- Real-time weather data for any city worldwide
- AI-powered natural language weather reports
- Temperature in Celsius with feels-like metrics
- Personalized clothing and activity recommendations
- Sunrise/sunset times and humidity tracking

### 2. **Interest-Based News Aggregator**
- Fetches latest news on topics you care about
- AI-powered news summarization using Gemini
- Visual news feed with images
- Direct links to full articles
- 5 top headlines with instant summaries

### 3. **Intelligent Day Planner**
- Context-aware itinerary generation
- Integrates weather forecast, local events, and tourist attractions
- Chronological planning (Morning → Afternoon → Evening)
- Indoor/outdoor activity recommendations based on weather
- Event discovery with timing and venue details
- Balanced schedule with sightseeing, food, and entertainment

### 4. **Daily Inspiration**
- Curated motivational quotes
- Beautiful morning imagery from Unsplash
- Clean, minimalist interface

## 🛠️ Technology Stack

- **Frontend:** Streamlit
- **AI/ML:** Google Gemini 2.5 Flash & Flash Lite
- **APIs:**
  - OpenWeather API (Weather data)
  - NewsAPI (News aggregation)
  - SerpAPI (Event discovery)
  - Google Search Grounding (Real-time information)
- **Languages:** Python 3.8+

## 📋 Prerequisites

- Python 3.8 or higher
- Google Gemini API key
- OpenWeather API key
- NewsAPI key
- SerpAPI key

## 🚀 Installation

1. **Clone the repository**
```bash
git clone https://github.com/Vishal-AI-ML/Morning-Buddy.git
cd Morning-Buddy
```

2. **Create virtual environment**
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install dependencies**
```bash
pip install -r requirements.txt
```

4. **Set up environment variables**

Create a `.env` file in the root directory:
```env
GOOGLE_API_KEY=your_gemini_api_key_here
```

5. **Update API keys in `applications.py`**
```python
# Weather API (line 28)
api_key="your_openweather_api_key"

# News API (line 73)
api_key="your_newsapi_key"

# Events API (line 125)
api_key="your_serpapi_key"
```

## 🎯 Usage

1. **Start the application**
```bash
streamlit run app.py
```

2. **Navigate through features**
   - **Home:** Get daily inspiration with quotes and images
   - **Weather:** Enter your city for AI-powered weather insights
   - **News:** Specify interests (e.g., Technology, Sports, Health)
   - **Smart Planner:** Generate complete day itinerary for any city

## 📁 Project Structure

```
Morning-Buddy/
├── app.py                 # Streamlit UI and page routing
├── applications.py        # Core AI functions and API integrations
├── .env                   # Environment variables (create this)
├── requirements.txt       # Python dependencies
└── README.md             # Project documentation
```

## 🔑 Key Functions

### `temperature_of_city(city)`
Fetches weather data and generates human-friendly reports with actionable recommendations.

### `get_news(topic)` & `news_summarizer(url)`
Retrieves latest news articles and creates concise AI summaries.

### `smart_plan(city)`
Orchestrates weather forecasts, events, and attractions into a personalized daily itinerary.

### `get_forcasted_weather(city)`
Uses Google Search grounding for real-time weather predictions and tourist recommendations.

### `find_local_events(city)`
Discovers upcoming events with timing, venue, and booking links.

## 🎨 UI Features

- **Multi-page navigation** via sidebar
- **Responsive design** with columns for news display
- **Random quote generator** for daily motivation
- **Dynamic image loading** from Unsplash
- **Clean markdown formatting** for readability

## 📊 API Rate Limits

| API | Free Tier Limit |
|-----|----------------|
| OpenWeather | 1,000 calls/day |
| NewsAPI | 100 requests/day |
| SerpAPI | 100 searches/month |
| Gemini | 15 RPM (requests per minute) |

## 👤 Author

**Vishal Shivhare**
- GitHub: [@Vishal-AI-ML](https://github.com/Vishal-AI-ML)
- LinkedIn: [Vishal Shivhare](https://linkedin.com/in/vishal-shivhare-562508243)
- Email: vishalshivhare.ai@gmail.com

## 🙏 Acknowledgments

- Google Gemini for powerful AI capabilities
- OpenWeather, NewsAPI, and SerpAPI for data services
- Unsplash for beautiful imagery
- Streamlit for the amazing framework

⭐ **If you found this project helpful, please consider giving it a star!**

**Made with ❤️ and ☕ by Vishal Shivhare**
