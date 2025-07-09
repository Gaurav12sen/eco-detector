# ♻️ Eco Detector – Smart Scrap Classifier

[Live Demo](https://eco-detector.streamlit.app/)

## Overview

Eco Detector is an AI-powered web application that helps users classify scrap items for recycling and resale. By uploading images of scrap items, users receive instant, location-specific guidance on recyclability, potential scrap value, preparation steps, safety guidelines, and environmental impact. The app leverages Google Gemini AI for image analysis and provides local recycling rules tailored to Indian states.

---

## Features

- **AI Scrap Classification:**  
  Upload images of scrap items (plastic, metal, e-waste, etc.) and get an AI-generated analysis.
- **Location-Aware Guidance:**  
  Detects your location (via browser or manual input) to provide state-specific recycling rules and recommendations.
- **Recyclability & Value Estimation:**  
  Tells you if the item is recyclable and estimates its potential resale value.
- **Preparation & Safety Tips:**  
  Offers actionable steps to prepare items for recycling and safe handling.
- **Environmental Impact:**  
  Explains the environmental benefits of recycling each item.
- **User-Friendly Interface:**  
  Clean, interactive UI with animations and clear instructions.

---

## How It Works

1. **Set Your Location:**  
   - Use the "Detect My Location" button for automatic detection, or manually select your city and state.
2. **Upload Images:**  
   - Upload one or more images of your scrap items (supported formats: JPG, JPEG, PNG, WEBP).
3. **Get Instant Analysis:**  
   - The app analyzes each item and displays:
     - Recyclability (based on local rules)
     - Estimated scrap value
     - Preparation steps
     - Safety guidelines
     - Environmental impact
4. **Review Local Recycling Rules:**  
   - View state-specific recycling guidelines in the sidebar or expander.

---

## Technologies Used

- **Streamlit:** For building the interactive web app.
- **Google Gemini (Generative AI):** For image-based scrap classification and analysis.
- **Geolocation:** Uses browser geolocation and manual override for location-aware recommendations.
- **Pillow:** For image processing.
- **Bokeh & Streamlit-Bokeh-Events:** For browser-based geolocation integration.
- **Lottie Animations:** For engaging UI elements.

---

## Setup & Installation

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/eco-detector.git
cd eco-detector
```

### 2. Install Dependencies

Make sure you have Python 3.8+ installed.

```bash
pip install -r requirements.txt
```

### 3. Set Up API Key

- Obtain a Google Generative AI API key (Gemini).
- Create a `.env` file in the project root:

  ```
  API_KEY=your_actual_api_key_here
  ```

### 4. Run the App Locally

```bash
python -m streamlit run app.py
```

The app will open in your browser at `http://localhost:8501`.

---

## Usage

- Use the sidebar to set your location and upload images.
- Review the AI-generated analysis and follow the preparation and safety tips.
- Check the local recycling rules for your state.

---

## Environment Variables

- `API_KEY` – Your Google Generative AI (Gemini) API key.  
  Must be set in a `.env` file in the project root.

---

## File Structure

- `app.py` – Main Streamlit app.
- `waste_info.py` – Contains waste classification logic and recycling rules.
- `geo_location.py` – Handles browser-based geolocation.
- `requirements.txt` – Python dependencies.
- `README.md` – Project documentation.

---

## Contributing

Contributions are welcome! Please open issues or submit pull requests for improvements or new features.

---

## License

MIT License (add a LICENSE file if you want to specify a license)

---

## Acknowledgements

- Google Generative AI (Gemini)
- Streamlit Community
- OpenStreetMap Nominatim (for reverse geocoding)
- LottieFiles (for animations)
