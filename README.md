# 🩸 Period Tracker

A modern, secure period tracking application built with ASP.NET Core MVC for educational purposes.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![.NET](https://img.shields.io/badge/.NET-6.0-purple.svg)](https://dotnet.microsoft.com/download/dotnet/6.0)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)

## 📋 Table of Contents

- [About](#about)
- [Features](#features)
- [Screenshots](#screenshots)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Configuration](#configuration)
- [Usage](#usage)
- [Contributing](#contributing)
- [Privacy & Security](#privacy--security)
- [License](#license)
- [Contact](#contact)

## 🎯 About

Period Tracker is a comprehensive menstrual cycle tracking application developed as an educational project to demonstrate modern web development practices using ASP.NET Core MVC. The application focuses on user privacy, data security, and an intuitive user experience.

**⚠️ Educational Project Notice**: This project is developed for educational purposes as part of an ASP.NET Core MVC learning exercise.

## ✨ Features

- 🔐 **Secure Authentication**
  - Facebook OAuth integration
  - Google OAuth integration
  - Secure session management

- 📊 **Comprehensive Tracking**
  - Menstrual cycle logging
  - Symptom tracking
  - Mood monitoring
  - Cycle predictions

- 📱 **User Experience**
  - Responsive design for all devices
  - Intuitive dashboard
  - Data visualization
  - Export functionality

- 🔒 **Privacy & Security**
  - Data encryption
  - Secure authentication
  - GDPR compliant
  - No data sharing with third parties

## 📸 Screenshots

> **Note**: Screenshots will be added as the project develops.

## 🛠 Tech Stack

**Backend:**
- ASP.NET Core 6.0 MVC
- Entity Framework Core
- SQL Server
- Identity Framework

**Frontend:**
- HTML5, CSS3, JavaScript
- Bootstrap 5
- Chart.js (for data visualization)

**Authentication:**
- Facebook OAuth 2.0
- Google OAuth 2.0

**Deployment:**
- Azure App Service (planned)
- Azure SQL Database (planned)

## 🚀 Getting Started

### Prerequisites

Before you begin, ensure you have the following installed:
- [.NET 6.0 SDK](https://dotnet.microsoft.com/download/dotnet/6.0)
- [Visual Studio 2022](https://visualstudio.microsoft.com/) or [Visual Studio Code](https://code.visualstudio.com/)
- [SQL Server](https://www.microsoft.com/en-us/sql-server/sql-server-downloads) or [SQL Server Express](https://www.microsoft.com/en-us/sql-server/sql-server-editions-express)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/period-tracker.git
   cd period-tracker
   ```

2. **Restore NuGet packages**
   ```bash
   dotnet restore
   ```

3. **Set up the database**
   ```bash
   dotnet ef database update
   ```

4. **Configure authentication** (see [Configuration](#configuration) section)

5. **Run the application**
   ```bash
   dotnet run
   ```

6. **Open your browser** and navigate to `https://localhost:5001`

### Quick Start with Docker (Optional)

```bash
# Clone the repository
git clone https://github.com/yourusername/period-tracker.git
cd period-tracker

# Run with Docker Compose
docker-compose up -d
```

## ⚙️ Configuration

### Authentication Setup

#### Facebook OAuth
1. Create a Facebook App at [Facebook Developers](https://developers.facebook.com/)
2. Get your App ID and App Secret
3. Add to `appsettings.json`:
   ```json
   {
     "Facebook": {
       "AppId": "your-facebook-app-id",
       "AppSecret": "your-facebook-app-secret"
     }
   }
   ```

#### Google OAuth
1. Create credentials at [Google Cloud Console](https://console.cloud.google.com/)
2. Get your Client ID and Client Secret
3. Add to `appsettings.json`:
   ```json
   {
     "Google": {
       "ClientId": "your-google-client-id",
       "ClientSecret": "your-google-client-secret"
     }
   }
   ```

### Database Configuration

Update the connection string in `appsettings.json`:
```json
{
  "ConnectionStrings": {
    "DefaultConnection": "Server=(localdb)\\mssqllocaldb;Database=PeriodTrackerDb;Trusted_Connection=true;MultipleActiveResultSets=true"
  }
}
```

### Environment Variables (Recommended for Production)

For better security, use environment variables:
```bash
export FACEBOOK_APP_ID="your-facebook-app-id"
export FACEBOOK_APP_SECRET="your-facebook-app-secret"
export GOOGLE_CLIENT_ID="your-google-client-id"
export GOOGLE_CLIENT_SECRET="your-google-client-secret"
```

## 📖 Usage

### For Users

1. **Sign Up/Login**: Use Facebook or Google to create an account
2. **Track Cycles**: Log your menstrual cycle data
3. **Monitor Symptoms**: Record symptoms and moods
4. **View Analytics**: Check your cycle patterns and predictions
5. **Export Data**: Download your data for personal records

### For Developers

This project demonstrates:
- OAuth 2.0 implementation with multiple providers
- Entity Framework Core with migrations
- MVC pattern implementation
- Responsive web design
- Data visualization with Chart.js
- Security best practices

## 🤝 Contributing

We welcome contributions! This is an educational project, so it's a great opportunity to learn and collaborate.

### How to Contribute

1. **Fork the repository**
2. **Create a feature branch**
   ```bash
   git checkout -b feature/AmazingFeature
   ```
3. **Commit your changes**
   ```bash
   git commit -m 'Add some AmazingFeature'
   ```
4. **Push to the branch**
   ```bash
   git push origin feature/AmazingFeature
   ```
5. **Open a Pull Request**

### Contribution Guidelines

- Follow existing code style and conventions
- Write clear commit messages
- Add comments for complex logic
- Update documentation as needed
- Test your changes thoroughly

### Development Setup

```bash
# Install development tools
dotnet tool install --global dotnet-ef
dotnet tool install --global dotnet-aspnet-codegenerator

# Run in development mode
dotnet run --environment Development
```

## 🔒 Privacy & Security

This application takes privacy seriously:

- **Data Encryption**: All sensitive data is encrypted
- **Secure Authentication**: Industry-standard OAuth 2.0
- **No Data Sharing**: Your data is never shared with third parties
- **Educational Purpose**: Data used only for learning purposes
- **Right to Deletion**: Users can request data deletion

For full privacy details, see our [Privacy Policy](privacy-policy.html).

## 📋 Roadmap

- [ ] Mobile app (React Native)
- [ ] Advanced analytics and insights
- [ ] Export to various formats (PDF, CSV)
- [ ] Reminder notifications
- [ ] Multi-language support
- [ ] Dark mode theme
- [ ] API for third-party integrations

## 🐛 Known Issues

- None currently reported

## 📊 Project Status

This project is actively developed as part of an educational curriculum. Features are being added incrementally as learning progresses.

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Authors

- **Michael Ajayi** - *Initial work* - [@yourusername](https://github.com/yourusername)

## 🙏 Acknowledgments

- ASP.NET Core documentation and community
- Bootstrap for responsive design components
- Chart.js for data visualization
- Educational institution and instructors
- Open source community for inspiration

## 📞 Contact

- **Project Link**: [https://github.com/yourusername/period-tracker](https://github.com/yourusername/period-tracker)
- **Educational Institution**: [Your School Name]
- **Course**: ASP.NET Core MVC Development

## 📚 Additional Resources

- [ASP.NET Core Documentation](https://docs.microsoft.com/en-us/aspnet/core/)
- [Entity Framework Core Documentation](https://docs.microsoft.com/en-us/ef/core/)
- [OAuth 2.0 Specification](https://oauth.net/2/)
- [Bootstrap Documentation](https://getbootstrap.com/docs/)

---

⭐ **Star this repository if this project helped you learn something new!**

**Disclaimer**: This is an educational project. For production use, please ensure proper security audits and compliance with local regulations regarding health data.
