# Weather Dashboard

A modern, responsive weather dashboard application that fetches real-time weather data from the OpenWeatherMap API.

## Features

✨ **Core Features:**
- 🌍 Real-time weather data for any city worldwide
- 📍 Geolocation support to get weather for current location
- 🌡️ Current temperature and "feels like" temperature
- 💧 Humidity, wind speed, pressure, and visibility
- ☀️ UV Index information
- 🔄 5-day weather forecast
- 🎨 Modern, animated UI with gradient backgrounds
- 📱 Fully responsive design for mobile, tablet, and desktop
- ⚡ Fast and smooth animations
- 🛡️ Error handling and user-friendly messages

## Tech Stack

- **HTML5** - Semantic markup structure
- **CSS3** - Modern styling with gradients, animations, and flexbox/grid
- **JavaScript (ES6+)** - Async/await for API calls, DOM manipulation
- **OpenWeatherMap API** - Real-time weather data provider
- **Font Awesome** - Weather and UI icons

## Setup Instructions

### 1. Get OpenWeatherMap API Key

1. Go to [OpenWeatherMap](https://openweathermap.org/api)
2. Sign up for a free account
3. Generate an API key from your account dashboard
4. The free tier includes:
   - Current weather data
   - 5-day forecast
   - UV Index data

### 2. Configure API Key

Open `weather-app.js` and replace the API_KEY placeholder:

```javascript
const API_KEY = 'YOUR_OPENWEATHERMAP_API_KEY';
```

### 3. Open the Dashboard

Simply open `weather.html` in your web browser. No build process or server required for basic functionality!

## File Structure

```
├── weather.html          # Main HTML file with dashboard structure
├── weather-style.css     # Styling and animations
├── weather-app.js        # JavaScript logic and API integration
└── WEATHER_README.md     # This file
```

## How to Use

1. **Search by City**: Type a city name and click the Search button or press Enter
2. **Use Current Location**: Click the location icon to get weather for your current coordinates
3. **View Details**: See current temperature, conditions, humidity, wind speed, pressure, visibility, and UV index
4. **Check Forecast**: Browse the 5-day forecast at the bottom

## API Endpoints Used

1. **Current Weather**
   ```
   GET /weather?q={city}&units=metric&appid={API_KEY}
   GET /weather?lat={lat}&lon={lon}&units=metric&appid={API_KEY}
   ```

2. **UV Index**
   ```
   GET /uvi?lat={lat}&lon={lon}&appid={API_KEY}
   ```

3. **5-Day Forecast**
   ```
   GET /forecast?lat={lat}&lon={lon}&units=metric&appid={API_KEY}
   ```

## Features Breakdown

### Current Weather Display
- City name and country code
- Current temperature with color-coded icon
- Weather description
- Feels-like temperature
- Current date and day

### Weather Details
- **Humidity**: Current air humidity percentage
- **Wind Speed**: Wind speed in meters per second
- **Pressure**: Atmospheric pressure in hPa
- **Visibility**: Visibility range in kilometers
- **UV Index**: UV radiation intensity

### 5-Day Forecast
- One forecast card per day
- Temperature for the day
- Weather icon
- Weather description
- Smooth hover animations

## Responsive Design

The dashboard is optimized for:
- 📱 Mobile phones (320px and up)
- 📱 Tablets (768px and up)
- 💻 Desktop screens (1024px and up)

Media queries adjust:
- Font sizes
- Grid layouts
- Card sizes
- Button layouts

## Error Handling

The app includes comprehensive error handling for:
- City not found
- Invalid API key
- Network connectivity issues
- Geolocation permission denied
- API response errors

## Browser Compatibility

- Chrome/Edge (Latest)
- Firefox (Latest)
- Safari (Latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Performance Optimizations

- Minimal external dependencies
- Efficient DOM updates
- CSS animations instead of JavaScript animations
- Icon lazy loading
- Optimized API requests

## Future Enhancements

🚀 Potential features to add:
- Multiple city comparison
- Weather alerts
- Air quality index (AQI)
- Hourly forecast
- Weather history/trends
- Local storage for favorite cities
- Dark/light theme toggle
- Unit conversion (Celsius/Fahrenheit)
- Precipitation probability
- Sunrise/sunset times

## Troubleshooting

### "City not found"
- Ensure you're using the correct city name
- Try using a city name with country code (e.g., "London, UK")

### "Invalid API key"
- Verify your API key is correct in weather-app.js
- Check that your API key hasn't expired
- Generate a new API key from OpenWeatherMap

### Data not loading
- Check your internet connection
- Open browser console (F12) to see error messages
- Verify OpenWeatherMap API status

### Geolocation not working
- Check browser permissions for location access
- Ensure you're accessing the page over HTTPS (for security)
- Some browsers require explicit permission grants

## License

This project is open source and available for personal and commercial use.

## Resources

- [OpenWeatherMap API Documentation](https://openweathermap.org/api)
- [Font Awesome Icons](https://fontawesome.com/)
- [MDN Web Docs - Geolocation API](https://developer.mozilla.org/en-US/docs/Web/API/Geolocation_API)
- [MDN Web Docs - Fetch API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API)

---

**Created with ❤️ for weather enthusiasts and developers**