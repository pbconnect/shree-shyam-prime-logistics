# Shree Shyam Prime Logistics – Complete Starter

## Included
- Customer booking page
- Mahindra Veero 10 Feet vehicle
- Automatic fare calculation
- Booking API + local JSON storage
- Driver app starter
- Admin dashboard starter
- WhatsApp booking button
- Firebase configuration template for OTP + live GPS/realtime tracking

## Run
1. Install Node.js.
2. Open this folder in terminal.
3. Run `npm install`
4. Run `npm start`
5. Open `http://localhost:3000`
6. Customer: `/`
7. Driver: `/driver.html`
8. Admin: `/admin.html`

## Production integrations to complete
### Google Maps
Create a Google Cloud project, enable Maps JavaScript API + Places + Routes/Distance Matrix as applicable, create an API key, restrict the key by domain, and add the Maps script to `public/index.html`. Then replace manual KM with route distance returned by Google Maps.

### Firebase
Create a Firebase project and Web App. Enable Phone Authentication and Realtime Database/Firestore. Copy values from `config/firebase-config.example.js` into `firebase-config.js`. Use Firebase Auth for OTP and Realtime Database for driver location/booking status.

### Admin security
For production, add admin authentication and server-side authorization. Never expose service-account keys in browser code.

### Fare model
Current demo:
base ₹500 + ₹35/km + loading/unloading + waiting; minimum ₹500.
Change the pricing object in `public/index.html`, or move it to the database/admin panel for live changes.

### WhatsApp
Replace `919999999999` in `public/index.html` with the company's WhatsApp number.

This is a starter implementation inspired by common logistics-app flows. It does not copy Porter's proprietary code, branding, or private APIs.
