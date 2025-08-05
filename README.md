# Period Tracker

A simple period tracking web application built with ASP.NET Core MVC for educational purposes.

## About

This is a student project demonstrating:
- ASP.NET Core MVC development
- Facebook and Google OAuth authentication
- Entity Framework Core
- Responsive web design

## Features

- 🔐 Login with Facebook or Google
- 📊 Track menstrual cycles
- 📱 Mobile-friendly design
- 🔒 Secure data storage

## Getting Started

### Prerequisites
- .NET 6.0 SDK
- Visual Studio or VS Code
- SQL Server

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/period-tracker.git
   cd period-tracker
   ```

2. Restore packages:
   ```bash
   dotnet restore
   ```

3. Update database:
   ```bash
   dotnet ef database update
   ```

4. Add your OAuth credentials to `appsettings.json`:
   ```json
   {
     "Facebook": {
       "AppId": "your-facebook-app-id",
       "AppSecret": "your-facebook-app-secret"
     },
     "Google": {
       "ClientId": "your-google-client-id",
       "ClientSecret": "your-google-client-secret"
     }
   }
   ```

5. Run the application:
   ```bash
   dotnet run
   ```

## Tech Stack

- **Backend**: ASP.NET Core 6.0 MVC
- **Database**: Entity Framework Core with SQL Server
- **Authentication**: Facebook OAuth, Google OAuth
- **Frontend**: HTML, CSS, JavaScript, Bootstrap

## Contributing

This is an educational project. Pull requests and suggestions are welcome!

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## Privacy

This application collects minimal data for educational purposes only. See [Privacy Policy](privacy-policy.html) for details.

## License

MIT License - see [LICENSE](LICENSE) file for details.

## Contact

- **Developer**: Michael Ajayi
- **Project**: Educational ASP.NET Core MVC demonstration

---

**Note**: This is a student project for learning purposes.
