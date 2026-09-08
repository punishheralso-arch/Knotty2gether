# Knotty2gether Frontend

React-based web application for:
- Client registration and authentication
- Experience booking interface
- Payment processing with Stripe
- Video submission and confirmation
- Session tracking and management
- Admin dashboard for creator

## Tech Stack

- **Framework**: React 18+
- **Build**: Vite
- **State Management**: Redux Toolkit
- **Styling**: Tailwind CSS
- **Form Handling**: React Hook Form
- **Payments**: Stripe React Library
- **HTTP**: Axios
- **Video**: AWS S3 integration

## Setup

```bash
npm install
cp .env.example .env
npm run dev
```

## Project Structure

```
frontend/
├── src/
│   ├── components/
│   │   ├── Auth/
│   │   │   ├── Register.jsx
│   │   │   └── Login.jsx
│   │   ├── Booking/
│   │   │   ├── BookingForm.jsx
│   │   │   ├── ExperienceSelector.jsx
│   │   │   └── DatePicker.jsx
│   │   ├── Payment/
│   │   │   ├── PaymentForm.jsx
│   │   │   └── StripeCheckout.jsx
│   │   ├── VideoConfirmation/
│   │   │   ├── VideoUpload.jsx
│   │   │   └── ConfirmationStatus.jsx
│   │   └── Dashboard/
│   │       ├── ClientDashboard.jsx
│   │       └── AdminDashboard.jsx
│   ├── pages/
│   │   ├── Home.jsx
│   │   ├── BookingPage.jsx
│   │   ├── PaymentPage.jsx
│   │   └── DashboardPage.jsx
│   ├── store/
│   │   ├── authSlice.js
│   │   ├── bookingSlice.js
│   │   └── store.js
│   ├── services/
│   │   ├── api.js
│   │   ├── authService.js
│   │   ├── bookingService.js
│   │   └── paymentService.js
│   ├── App.jsx
│   └── main.jsx
├── public/
├── .env.example
├── vite.config.js
├── package.json
└── tailwind.config.js
```

## Key Features

### Booking Flow
1. Client registers/logs in
2. Selects experience type (couples or nudist)
3. Chooses date/time
4. Reviews pricing
5. Proceeds to payment

### Payment Integration
- Stripe payment intent creation
- Secure card processing
- Confirmation and receipt

### Video Confirmation
- Presigned S3 upload URL
- Video submission tracking
- Status updates and feedback

### Admin Dashboard
- Booking management
- Video review interface
- Client verification
- Session tracking

---

**Last Updated**: 2026-09-07
