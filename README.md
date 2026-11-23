==============================
Desi-Mochi or Mochi-Keychain =
==============================

Version 1.2
* Modularized the Code
* Background Effects have random spead and patterns based on each expression
* Add LOVING Expression with Heart beat pattern, the eye and mouth are Heart Shaped

Version 1.3
* Adding Indian character symbols like Shiva's Third Eye with falling Trishul streams, Hanuman's Energetic Tilak,
    Vishnu's Royal tilak, and Brahma's Crown arcs cascading with sacred aura backgrounds.

Version 1.3.1:
* Add Speaker/Buzzer to the Project - GPIO2
* Added HappyBirthday tune, and this possible with Active Buzzer speaker

Version 1.3.2:
* Add touch Sensor TTP223
* Introduced a Menu with Modular tabs to choose different settings. One touch navigate through menus and Long touch
    to select the option, One touch then to change values, again Long touch to de-select the option.

Version 1.4:
* Adding advanced features like CLOCK + WEATHER + FACE Modes
* Touch State Engine as below:
    - Triple Tap: Toggles the Settings Menu
    - Double Tap: Instantly rotates to next application screen (Face -> Smart Clock -> Weather Forecast -> Face)/
    - Single Tap: Moves Rows inside the Menu (if Menu is Open) or Triggers a saccade eye roll look-around (if Menu is Closed)

Version 1.4.1:
* Add Automatic sync of time and weather from NTP and Openweather API
// =======================================================
// --- USER CONFIGURABLE WIFI & API CREDENTIALS ---
// =======================================================
#define WIFI_SSID       "ACT_AAFD"      // Replace with your home WiFi router name
#define WIFI_PASSWORD   "BNFhX8iF"  // Replace with your WiFi password
#define WEATHER_API_KEY "7f07bc20c4ed3656f52e47351a7e74c2"   // Replace with your OpenWeatherMap free API key
#define WEATHER_CITY    "Bengaluru,IN"        // Format: "CityName,CountryCode"
// =======================================================

  // --- NEW WEATHERAPI.COM SECURE API PATH ENDPOINT ---
    #define WEATHER_API_KEY "e64a6d1a9e224526a52180347261108" 
    #define WEATHER_CITY    "Bengaluru" 
  String serverPath = "https://api.weatherapi.com/v1/current.json?key=" + String(WEATHER_API_KEY) + "&q=" + cityQuery + "&aqi=no";
    //https://api.weatherapi.com/v1/current.json?key=e64a6d1a9e224526a52180347261108&q=Bengaluru&aqi=no

Version 1.5:
* Make WiFi configuration Dynamic
* Fixed the Weather Text to display in two rows towards right bottom side
* Fixed Wifi connection with AP (Accesspoint) and move on to live mode.
* Added Brightness control in Settings Menu.
* Fixed SSD1306 hardware compatible along with SH1106 code bug
* Auto adjust brighness to 10% upon idle for a minute, means no touch.

Version 1.6:
* Enable OTA (Over the Air) functionality.
  String serverPath = "https://api.weatherapi.com/v1/current.json?key=" + String(WEATHER_API_KEY) + "&q=" + cityQuery + "&aqi=no";
* Enhance the WiFi Captive Portal webpage with scanning available 2.4GHz access points (SSID) to choose while wifi setup.
* Enable Github Software Update Function.  This will use OTA to update teh Software from Github.

That is awesome news! Everything is officially up and running—Desi-Mochi-Setup Wi-Fi scanning, NTP clock synchronization, 
ive weather forecasts, 16 custom animated expressions, idle brightness dimming, and one-click GitHub Cloud OTA updates are 
all working together smoothly.

Version 1.6.1:
* Add Reset Wi-Fi option to the settings Menu.
* Add About option to the Settings Menu.
  - This will display Product name, OS Version, WiFi Name, Signal Quality/Strength, Local IP Address.

Version 1.6.2:
* OLED: Menu Option to Dynamic select between SH1106 and SSD1306 screen types
* an Introduction Splash screen with Logo 'M' + Matomation text

Version 1.7.0:
* Adding Snake Game of Nokia basic phone

Version 1.7.1:
* Adding 20 more faces with special Clock face

Version 1.8.0
* Adding Music functionality
  - Western Songs
  - Carnatic Songs
  - Tone
  - Tempo

Version 1.9.1
* Adding HTTP Settings Webpage to control the device from Smartphone/Laptop
String dynamicUrl = "https://api.weatherapi.com/v1/current.json?key=" + String(WEATHER_API_KEY) + "&q=" + encodedCity + "&aqi=no";
* Change Company name from Matomation to M2 Automations and also the Logo
* Add new game Flappy Buddy.
