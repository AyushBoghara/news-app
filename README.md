# News App

[![Android](https://img.shields.io/badge/Platform-Android-green.svg)](https://developer.android.com/)
[![API](https://img.shields.io/badge/API-24%2B-brightgreen.svg?style=flat)](https://android-arsenal.com/api?level=24)
[![Java](https://img.shields.io/badge/Language-Java-orange.svg)](https://www.java.com/)

A modern Android news application that fetches and displays the latest news articles from various categories using the NewsAPI. Built with Material Design principles and optimized for a smooth user experience.

## 📱 Features

- **Real-time News Fetching**: Get the latest news articles from NewsAPI
- **Category Filtering**: Browse news by categories (General, Business, Sports, Technology, etc.)
- **Search Functionality**: Search for specific news topics or keywords
- **Detailed Article View**: Read full articles with images and descriptions
- **Responsive Design**: Optimized for different screen sizes
- **Material Design UI**: Clean and intuitive user interface
- **Offline Caching**: View previously loaded articles without internet connection
- **Image Loading**: Efficient image loading and caching with Picasso

## 🛠️ Tech Stack

- **Language**: Java
- **Platform**: Android (API 24+)
- **Architecture**: MVC Pattern
- **Networking**: Retrofit 2.9.0
- **JSON Parsing**: Gson Converter
- **Image Loading**: Picasso 2.8
- **UI Components**: 
  - RecyclerView for news list
  - SearchView for search functionality
  - Material Design Components
  - ConstraintLayout for responsive layouts

## 📋 Prerequisites

Before you begin, ensure you have the following installed:

- Android Studio Arctic Fox or later
- Java Development Kit (JDK) 8 or higher
- Android SDK with API level 24 or higher
- NewsAPI key (free registration at [newsapi.org](https://newsapi.org/))

## 🚀 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/news-app.git
   cd news-app
   ```

2. **Open in Android Studio**
   - Launch Android Studio
   - Select "Open an existing Android Studio project"
   - Navigate to the cloned repository folder and select it

3. **Get NewsAPI Key**
   - Visit [NewsAPI.org](https://newsapi.org/)
   - Sign up for a free account
   - Copy your API key

4. **Configure API Key**
   - Open `app/src/main/res/values/strings.xml`
   - Replace `YOUR_API_KEY_HERE` with your actual NewsAPI key:
   ```xml
   <string name="api_key">your_actual_api_key_here</string>
   ```

5. **Sync Project**
   - Click "Sync Now" when prompted, or go to File → Sync Project with Gradle Files

6. **Build the Project**
   - Go to Build → Make Project or press `Ctrl+F9`

## 🎯 Usage

### Running the App

1. **Connect an Android device** or **start an emulator**
2. **Run the application**:
   - Click the "Run" button in Android Studio
   - Or use the keyboard shortcut `Shift+F10`
   - Or run via command line:
   ```bash
   ./gradlew installDebug
   ```

### App Navigation

1. **Home Screen**: Displays general news articles by default
2. **Category Buttons**: Tap any category button to filter news
3. **Search**: Use the search bar to find specific topics
4. **Article Details**: Tap any article to view full details
5. **Refresh**: Pull down to refresh the news feed

### Available Categories

- General
- Business
- Entertainment
- Health
- Science
- Sports
- Technology

## ⚙️ Configuration

### API Configuration

The app uses NewsAPI for fetching news data. Configuration is handled in:

- **API Key**: Set in `strings.xml`
- **Base URL**: Configured in `RequestManager.java`
- **Country Code**: Currently set to "in" (India) in `RequestManager.java`

### Customization Options

1. **Change Country**: Modify the country parameter in `RequestManager.java`
2. **Add Categories**: Update the category buttons in `activity_main.xml`
3. **Modify UI**: Customize layouts in the `res/layout/` directory
4. **Change Theme**: Update colors and styles in `res/values/`

### Network Configuration

Ensure your `AndroidManifest.xml` includes:
```xml
<uses-permission android:name="android.permission.INTERNET" />
```

## 🤝 Contributing

We welcome contributions to improve the News App! Here's how you can help:

### Getting Started

1. **Fork the repository**
2. **Create a feature branch**:
   ```bash
   git checkout -b feature/amazing-feature
   ```
3. **Make your changes**
4. **Commit your changes**:
   ```bash
   git commit -m 'Add some amazing feature'
   ```
5. **Push to the branch**:
   ```bash
   git push origin feature/amazing-feature
   ```
6. **Open a Pull Request**

### Contribution Guidelines

- Follow Android development best practices
- Write clear, commented code
- Test your changes thoroughly
- Update documentation as needed
- Follow the existing code style
- Add unit tests for new features

### Code Style

- Use meaningful variable and method names
- Follow Java naming conventions
- Add comments for complex logic
- Keep methods focused and concise

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


## 📞 Support

If you encounter any issues or have questions:

- Create an issue on GitHub
- Check existing issues for solutions
- Review the documentation

## 🔄 Version History

- **v1.0.0** - Initial release
  - Basic news fetching functionality
  - Category filtering
  - Search feature
  - Article detail view

## 🙏 Acknowledgments

- [NewsAPI](https://newsapi.org/) for providing the news data
- [Retrofit](https://square.github.io/retrofit/) for networking
- [Picasso](https://square.github.io/picasso/) for image loading
- Android community for continuous support and resources
  
## Contact
For any inquiries or support, please contact:
- **Developer:** Ayush M Boghara
- **Email:** [bogharaayush1124@gmail.com]
- **GitHub:** [AyushBoghara](https://github.com/AyushBoghara)
---

**Made with ❤️ for Ayush Boghara**
