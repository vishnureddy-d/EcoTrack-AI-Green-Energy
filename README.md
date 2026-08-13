# 🌱 EcoTrack: AI Green Energy Platform

An interactive web application that uses **Google Generative AI (Gemini)** to analyze your daily energy consumption and carbon footprint.

## Features

- **AI-Powered Activity Parsing**: Describe your day in natural language, and Gemini extracts energy metrics
- **Carbon Footprint Calculation**: Automatic CO₂ emissions calculation based on grid electricity, solar energy, and fuel usage
- **Interactive Visualizations**: Dynamic Plotly charts showing emission breakdowns
- **Green Energy Simulator**: Explore the impact of switching to solar power with a live slider simulator
- **Real-time Results**: Instant calculations and environmental impact metrics

## Installation

1. **Clone the repository:**
   ```bash
   git clone <your-repo-url>
   cd "Project files"
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up your API key:**
   - Create a `.env` file in the project directory:
     ```
     GOOGLE_API_KEY=your_gemini_api_key_here
     ```
   - Get your Gemini API key from: https://aistudio.google.com

4. **Run the app:**
   ```bash
   streamlit run app.py
   ```

The app will open at `http://localhost:8501`

## Deployment on Streamlit Cloud

1. **Push to GitHub:**
   ```bash
   git add .
   git commit -m "Prepare for Streamlit Cloud deployment"
   git push origin main
   ```

2. **Deploy on Streamlit Cloud:**
   - Go to https://share.streamlit.io
   - Sign in with your GitHub account
   - Click "New app"
   - Select your repository, branch (`main`), and file (`app.py`)
   - Click "Deploy"

3. **Add Secrets:**
   - In Streamlit Cloud app settings, go to **Secrets**
   - Add: `GOOGLE_API_KEY = your_gemini_api_key_here`
   - The app will automatically use this key

## Emission Factors Used

- **Grid Electricity**: 0.82 kg CO₂/kWh (coal-heavy traditional grid)
- **Solar Electricity**: 0.05 kg CO₂/kWh (lifecycle manufacturing emissions)
- **Petrol**: 2.31 kg CO₂/L
- **Diesel**: 2.68 kg CO₂/L

## Tech Stack

- **Streamlit**: Web framework
- **Google Generative AI (Gemini)**: AI parsing and analysis
- **Plotly**: Interactive visualizations
- **Python-dotenv**: Environment variable management

## License

MIT

## Contributing

Feel free to submit issues and enhancement requests!
