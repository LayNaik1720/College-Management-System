# College Management System

A comprehensive web-based College Management System built with ASP.NET Core MVC, Entity Framework Core, and SQL Server.

## Features

###  Authentication & Authorization
- Role-based access control (Admin, Teacher, HOD, Student)
- Secure login/logout functionality
- User registration system

###  Admin Features
- Manage users (Teachers, Students, HODs)
- System configuration
- Full access to all modules

###  Teacher Features
- View assigned courses
- Mark student attendance
- Generate reports
- Student management

### Student Features
- View enrolled courses
- Check attendance records
- View academic profile

### Additional Features
- Attendance tracking system
- Excel export functionality
- Email notifications
- Analytics and reporting

## Technology Stack

- **Backend**: ASP.NET Core MVC (.NET 9)
- **Database**: SQL Server with Entity Framework Core
- **Frontend**: HTML5, CSS3, Bootstrap, JavaScript
- **Authentication**: ASP.NET Core Identity
- **Email**: SMTP Email Service
- **Excel Export**: EPPlus Library

## Prerequisites

- .NET 9 SDK
- SQL Server (LocalDB or full version)
- Visual Studio 2022 or VS Code

## Installation & Setup

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd CollegeManagementSystem
   ```

2. **Update Connection String**
   - Open `appsettings.json`
   - Update the `DefaultConnection` string to match your SQL Server instance

3. **Install Dependencies**
   ```bash
   dotnet restore
   ```

4. **Run Database Migrations**
   ```bash
   dotnet ef database update
   ```

5. **Run the Application**
   ```bash
   dotnet run
   ```

6. **Access the Application**
   - Open browser and navigate to `https://localhost:
7.NOTE:
create a mvc using dotnet new mvc (project name) and just copy the required files form the repo to the project

## Default Login Credentials

### Admin Account
- **Email**: `admin@college.com`
- **Password**: `Admin@123`


## Project Structure

```
CollegeManagementSystem/
├── Controllers/           # MVC Controllers
├── Models/               # Data models and entities
├── Views/                # Razor views
├── Data/                 # Database context and migrations
├── Services/             # Business logic services
├── Utilities/            # Helper classes
├── wwwroot/              # Static files (CSS, JS, images)
├── Properties/           # Launch settings
└── appsettings.json      # Configuration file
```

## Key Models

- **ApplicationUser**: Base user model with Identity
- **Teacher**: Teacher-specific information
- **Student**: Student-specific information
- **Course**: Course management
- **Attendance**: Attendance tracking
- **Department**: Department management

## Configuration

### Database Configuration
Update `appsettings.json`:
```json
{
  "ConnectionStrings": {
    "DefaultConnection": "Server=(localdb)\\mssqllocaldb;Database=CollegeManagementDB;Trusted_Connection=true;MultipleActiveResultSets=true"
  }
}
```

### Email Configuration (Optional)
```json
{
  "SmtpSettings": {
    "Host": "smtp.gmail.com",
    "Port": "587",
    "User": "your-email@gmail.com",
    "Pass": "your-app-password"
  }
}
```

## Usage

1. **Login as Admin**
   - Use default admin credentials
   - Create departments, courses, and users

2. **Teacher Workflow**
   - Login with teacher credentials
   - View assigned courses
   - Mark attendance for students
   - Generate reports

3. **Student Workflow**
   - Login with student credentials
   - View enrolled courses
   - Check attendance records

## Features in Detail

### Attendance Management
- Teachers can mark daily attendance
- Students can view their attendance records
- Attendance percentage calculation
- Export attendance reports to Excel

### User Management
- Admin can create/edit/delete users
- Role assignment (Admin, Teacher, Student, HOD)
- Profile management

### Reporting
- Attendance reports
- Student performance analytics
- Excel export functionality

## Troubleshooting

### Common Issues

1. **Database Connection Error**
   - Ensure SQL Server is running
   - Check connection string in `appsettings.json`

2. **Migration Issues**
   ```bash
   dotnet ef migrations add InitialCreate
   dotnet ef database update
   ```

3. **Port Already in Use**
   - Change ports in `Properties/launchSettings.json`

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

This project is licensed under the MIT License.

## Support

For support and questions, please contact the development team or create an issue in the repository.

## Version History

- **v1.0.0** - Initial release with basic functionality
- Authentication system
- User management
- Attendance tracking
- Basic reporting

---

**Note**: This is an educational project designed for learning ASP.NET Core MVC development.
OUTPUT:
<img width="1919" height="1078" alt="Screenshot 2025-10-27 094947" src="https://github.com/user-attachments/assets/19b0982f-6053-47fb-881a-9c45de1baad0" />
<img width="1919" height="1079" alt="Screenshot 2025-10-27 095001" src="https://github.com/user-attachments/assets/bbfb41b8-ab18-4751-b515-6ae4d0cb5153" />
<img width="1919" height="1078" alt="Screenshot 2025-10-27 095011" src="https://github.com/user-attachments/assets/1b573e80-e06c-4c57-ba23-f5e952767fcc" />
<img width="1919" height="1079" alt="Screenshot 2025-10-27 095028" src="https://github.com/user-attachments/assets/df744683-4a99-4922-981e-e3e8eb6dc7f0" />
<img width="1919" height="1079" alt="Screenshot 2025-10-27 095042" src="https://github.com/user-attachments/assets/1044850a-8fb2-4895-adb1-b8d974f9ed3e" />
<img width="1915" height="1078" alt="Screenshot 2025-10-27 095101" src="https://github.com/user-attachments/assets/4755fd61-b422-4831-a035-ba2d37bc594b" />

