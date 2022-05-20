# TranzeetDashboard

# Tranzeet 

We are Moving The World Together because shaping the future of tranzportation is no accident Imagine First
<br>

# Inroduction
    TranZeet a platform that enables, freight owners and shippers to find carriers on the most suitable and rapid conditions; individual and corporate shippers to easily book freight for their return path via smartphones that displays the user’s transaction in interactive model using easy interface, for most existing delivery services.

---
## Technology Used
- Mobile Apps (IOS & Android) – React Native and Expo
- Admin Portal & Website – React and Redux
- Database – Firebase Realtime Database
- Server Side APIs – Firebase Cloud Functions
- Maps & Location APIs – Google
- Push Notifications – Expo



Notes: 
- The whole project has many sub projects. All the sub projects are working together by Monorepo concept.
    - Common (lib)
    - Functions (firebase functions)
    - Mobile App (React Native)
    - Website Admin (ReactJs)
        - Editing and Deleting on Admin Pages like Cart Types, Prices, Promos, etc are disabled in Admin Portal for Demo purposes.
        - Features like Email Verification, Driver Approval and Ride OTP are disabled for Demo purposes.


- React & React Native (Expo) 
- Database and Hosting – using the robust Firebase Realtime Database and Firebase’s own hosting platform. Firebase Fucntions are used for all the server side logic
- Authentication


## Technology Used
---
    Mobile Apps (IOS & Android) – React Native and Expo
    Admin Portal & Website – React and Redux
    Database – Firebase Realtime Database
    Server Side APIs – Firebase Cloud Functions
    Maps & Location APIs – Google
    Push Notifications – Expo

---
## Test Login App / Website 
https://tranzeet-it.web.app/login 

# Verification code
Role    Phone number      Verification code

Rider   +970 525000111    000000
Driver  +970 525000222    000000
Admin   +970 525000000    000000
## Test Payment Accounts
- Customer & Driver Account
    - Create directly on Apps (Use 2 different phones for Customer and Driver)
- Stripe testcard details
    - card no – 4242 4242 4242 4242 / cvv – Any 3 digits / exp date -Any future date
- Braintree testcard details
card no – 41111 1111 1111 1111 / cvv – Any 3 digits / exp date Any future date
- Paytm test credentials
    - Click here : https://developer.paytm.com/docs/testing-integration/
- Paystack testcard details
  - card no – 4084 0840 8408 4081 / cvv – 408 / exp date – Any future date
- Liqpay testcard details
    - card no – 4242 4242 4242 4242 / cvv – Any 3 digits / exp date – Any future date
- Flutterwave test cards
    - Click here [https://developer.flutterwave.com/docs/test-cards]
- SecurePay test cards
    - Click here [https://auspost.com.au/payments/docs/securepay/?javascript#securepay-api-card-payments-testing]
- Payu Latam and Culqi test card
    - card no – 4111 1111 1111 1111 / cvv – Any 3 digits / exp date – Any future date
- Mercdo Pago Test Cards
    - Test Cards [https://www.mercadopago.com.br/developers/en/guides/online-payments/mobile-checkout/testing]

---



Mobile App Hierarchy
```
├── AppCommon.js
├── app.config.js
├── App.js
├── assets
│   ├── fonts
│   ├── images 
│   ├── payment-icons
│   └── sounds
├── babel.config.js
├── config
│   ├── AppCat.js
│   ├── AppConfig.js
│   ├── FirebaseConfig.js
│   └── GoogleMapApiConfig.js
├── GoogleService-Info.plist
├── google-services.json
├── metro.config.js
├── package.json
└── src
    ├── common
    │   └── theme.js
    ├── components
    │   ├── Background.js
    │   ├── BookingModal.js
    │   ├── Button.js
    │   ├── DeliveryModal.js
    │   ├── GetPushToken.js
    │   ├── index.js
    │   ├── LoadingModal.js
    │   ├── MaterialButtonDark.js
    │   ├── OptionModal.js
    │   ├── OtpModal.js
    │   ├── PaymentWebView.js
    │   ├── promoComponent.js
    │   ├── register.js
    │   ├── ridelist.js
    │   ├── SideMenuHeader.js
    │   ├── SideMenu.js
    │   └── WalletTransactionHistory.js
    ├── navigation
    │   └── AppNavigator.js
    └── screens
        ├── About.js
        ├── AddMoney.js
        ├── AuthLoadingScreen.js
        ├── BookedCabScreen.js
        ├── ConvertDriver.js
        ├── DriverIncomeScreen.js
        ├── DriverRating.js
        ├── DriverTrips.js
        ├── EditProfile.js
        ├── index.js
        ├── LoginScreen.js
        ├── MapScreen.js
        ├── Notifications.js
        ├── OnlineChat.js
        ├── PaymentDetails.js
        ├── ProfileScreen.js
        ├── Registration.js
        ├── RideDetails.js
        ├── RideListScreen.js
        ├── SearchScreen.js
        ├── SelectGatewayScreen.js
        ├── WalletDetails.js
        └── WithdrawMoney.js
```

Web App Hierarchy

```
├── components
    │   ├── AlertDialog.js
    │   ├── Card
    │   │   ├── CardBody.js
    │   │   ├── CardFooter.js
    │   │   ├── CardHeader.js
    │   │   └── Card.js
    │   ├── CircularLoading.js
    │   ├── ConfirmationDialogRaw.js
    │   ├── CountryListSelect.js
    │   ├── CountrySelect.js
    │   ├── CustomButtons
    │   │   └── Button.js
    │   ├── CustomInput
    │   │   └── CustomInput.js
    │   ├── DashboardCard.js
    │   ├── Footer
    │   │   └── Footer.js
    │   ├── GoogleMapsAutoComplete.js
    │   ├── Grid
    │   │   ├── GridContainer.js
    │   │   └── GridItem.js
    │   ├── Header
    │   │   ├── Header.js
    │   │   └── HeaderLinks.js
    │   ├── InfoArea
    │   │   └── InfoArea.js
    │   ├── Map.js
    │   ├── Parallax
    │   │   └── Parallax.js
    │   ├── ResponsiveDrawer.js
    │   ├── Theme
    │   │   └── WebTheme.js
    │   ├── Typography
    │   │   ├── Danger.js
    │   │   ├── Info.js
    │   │   ├── Muted.js
    │   │   ├── Primary.js
    │   │   ├── Quote.js
    │   │   ├── Small.js
    │   │   ├── Success.js
    │   │   └── Warning.js
    │   └── UsersCombo.js
    ├── config
    │   ├── AppCat.js
    │   ├── FirebaseConfig.js
    │   └── GoogleMapApiConfig.js
    ├── index.js
    ├── lists
    │   ├── datelocales.json
    │   ├── google-api-supported-lang.json
    │   └── langlocales.json
    └── views
        ├── AboutUs.js
        ├── AddBookings.js
        ├── AddMoney.js
        ├── AppInformation.js
        ├── AppMenu.js
        ├── AuthLoading.js
        ├── BookingHistory.js
        ├── CancellationReasons.js
        ├── CarTypes.js
        ├── CreateAdmin.js
        ├── Dashboard.js
        ├── DriverEarning.js
        ├── Drivers.js
        ├── Earningreports.js
        ├── FleetAdmins.js
        ├── LandingPage.js
        ├── LanguageSetting.js
        ├── LoginPage.js
        ├── MyProfile.js
        ├── Notifications.js
        ├── PrivacyPolicy.js
        ├── Promos.js
        ├── ProtectedRoute.js
        ├── RegisterPage.js
        ├── Riders.js
        ├── Sections
        │   ├── ProductSection.js
        │   └── SectionDownload.js
        ├── Settings.js
        └── Withdraws.js
```
