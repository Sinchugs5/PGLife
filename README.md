# PGlife

A comprehensive web-based platform for managing student housing (PG accommodations) with user authentication, property listings, and interest tracking.

## Features

- **User Authentication** - Secure login/signup system
- **Property Listings** - Browse PG accommodations by city
- **Search & Filter** - Find properties by location and preferences
- **Interest Tracking** - Save and manage favorite properties
- **User Dashboard** - Personal profile and interested properties
- **Rating System** - Property ratings for cleanliness, food, and safety
- **Responsive Design** - Mobile-friendly interface

## Tech Stack

- **Frontend:** HTML5, CSS3, Bootstrap 4, JavaScript, jQuery
- **Backend:** PHP 7+
- **Database:** MySQL
- **Server:** Apache (XAMPP/WAMP)

## Installation

### Prerequisites
- XAMPP/WAMP/LAMP server
- PHP 7.0 or higher
- MySQL 5.6 or higher

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/Sinchugs5/PGLife.git
   cd PGlife
   ```

2. **Move to web server directory**
   ```bash
   # For XAMPP on Windows
   copy * C:\xampp\htdocs\PGlife\
   
   # For XAMPP on Linux/Mac
   cp -r * /opt/lampp/htdocs/PGlife/
   ```

3. **Start web server**
   - Start Apache and MySQL in XAMPP Control Panel
   - Or use command line: `sudo /opt/lampp/lampp start`

4. **Create database**
   - Open phpMyAdmin: `http://localhost/phpmyadmin`
   - Create database named `pglife`
   - Import the database file (contact developer for SQL file)

5. **Configure database connection**
   - Edit `includes/database_connect.php` if needed
   - Default settings: host=127.0.0.1, user=root, password="", database=pglife

6. **Access the application**
   ```
   http://localhost/PGlife/
   ```

## Project Structure

```
PGlife/
├── api/                    # API endpoints
│   ├── login_submit.php
│   ├── signup_submit.php
│   └── toggle_interested.php
├── css/                    # Stylesheets
├── img/                    # Images and assets
├── includes/               # PHP includes
│   ├── database_connect.php
│   ├── header.php
│   └── footer.php
├── js/                     # JavaScript files
├── index.php              # Homepage
├── property_list.php      # Property listings
├── property_detail.php    # Property details
├── dashboard.php          # User dashboard
└── logout.php            # Logout functionality
```

## Usage

1. **Homepage** - Search for PG accommodations by city
2. **Property Listings** - View available properties with filters
3. **User Registration** - Create account to save interests
4. **Property Details** - View detailed information and ratings
5. **Dashboard** - Manage profile and interested properties

## Database Schema

Key tables:
- `users` - User accounts and profiles
- `properties` - PG property listings
- `cities` - Available cities
- `interested_users_properties` - User interest tracking

## Contributing

1. Fork the repository
2. Create feature branch (`git checkout -b feature/new-feature`)
3. Commit changes (`git commit -am 'Add new feature'`)
4. Push to branch (`git push origin feature/new-feature`)
5. Create Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support



## Author

Developed by Sinchana


---
