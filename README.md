# weather-and-alert-system-automation
🌦 Weather & Alert System Automation

This workflow automatically checks the weather for Lahore, Pakistan using the OpenWeather One Call API. It retrieves real-time data like current temperature, conditions (rain, clear, cloudy), and alerts if available.

A Manual or Schedule Trigger starts the workflow.

The HTTP Request Node calls OpenWeather with Lahore’s latitude & longitude.

A Condition Node (IF) checks the weather response (e.g., if current.weather[0].main = "Rain").

If the condition matches, the workflow sends an alert (e.g., Slack message to self, or could be any channel like Telegram/Email).

This ensures you get notified automatically whenever specific weather conditions occur.
