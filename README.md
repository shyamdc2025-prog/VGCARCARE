# VSCARCARE — Car Service Mobile App Prototype

## Included
- Customer and Admin login pages
- Customer service catalogue
- Service booking form
- Date, visit count, mobile number and address
- Automatic unique service ID
- Bill calculation and payment method selection
- Customer booking history
- Admin dashboard
- Service-rate chart and service-mix chart
- Booking table
- Logout
- LocalStorage demo database
- MySQL database schema + sample data

## Run
Open `index.html` in a browser, or use VS Code Live Server.

### Demo login
Customer:
- Mobile: `9876543210`
- Password: `customer123`

Admin:
- Email: `admin@vscarcare.com`
- Password: `admin123`

## Database
Run `database/vscarcare.sql` in MySQL.

The browser prototype intentionally uses LocalStorage so it works without a backend. For production, replace the LocalStorage functions with REST API calls to a backend (Node/Express, PHP, Java/Spring Boot, etc.).

## Power BI
The admin dashboard contains a Power BI-style local chart using Chart.js so the demo runs immediately.
For a real Power BI deployment:
1. Use the MySQL `services` and `bookings` tables as the data source.
2. Build the report in Power BI.
3. Publish the report.
4. Embed it using the Power BI JavaScript SDK / secure embed flow.
5. Keep authentication and data access on the server; do not expose database credentials in frontend JavaScript.

## Design references
The UI direction was informed by contemporary vehicle-service booking patterns such as MechConnect, Vehicle Doctor and automotive booking form examples. The implementation here is original HTML/CSS/JS.
