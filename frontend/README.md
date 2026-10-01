# IIIT Badminton Court Booking Frontend

A beautiful React frontend for the IIIT Badminton Court Booking System with OTP verification, college email validation, and smooth animations.

## Features

- 🎨 **Beautiful UI**: Modern design with Tailwind CSS and smooth animations
- 🔐 **OTP Verification**: Email-based verification for IIIT students
- 🏫 **College Email Validation**: Only @gmail.com emails allowed
- 📅 **Interactive Calendar**: Week view with color-coded slot status
- 🏸 **Smart Booking**: Game mode selection (singles/doubles) with sub-court booking
- 👨‍💼 **Admin Dashboard**: Create and manage court slots
- 📱 **Responsive Design**: Works perfectly on all devices
- ⚡ **Fast & Smooth**: Built with Vite and Framer Motion

## Setup Instructions

### 1. Install Dependencies
```bash
npm install
```

### 2. Create Environment File
Create a `.env.local` file in the frontend directory with:
```env
VITE_API_URL=http://localhost:4000
```

### 3. Start Development Server
```bash
npm run dev
```

The app will open at `http://localhost:5173`

## Tech Stack

- **Frontend**: React 18 + Vite
- **Styling**: Tailwind CSS
- **Animations**: Framer Motion
- **Icons**: Lucide React
- **HTTP Client**: Axios
- **Routing**: React Router DOM

## Project Structure

```
src/
├── components/
│   ├── LoadingSpinner.jsx    # Beautiful loading animation
│   ├── Navbar.jsx            # Navigation with user menu
│   └── BookingModal.jsx      # Slot booking modal
├── pages/
│   ├── LoginPage.jsx         # Login/Register with OTP
│   ├── CalendarPage.jsx      # Main calendar view
│   └── AdminPage.jsx         # Admin slot creation
├── App.jsx                   # Main app with routing
└── main.jsx                  # App entry point
```

## Usage

### For Students
1. **Register**: Use your @gmail.com email
2. **Verify Email**: Enter the OTP sent to your email
3. **Login**: Access the booking system
4. **Book Slots**: Select date, time, and sub-court
5. **Choose Game Mode**: Singles (2 players) or Doubles (4 players)

### For Admins
1. **Login**: Use admin credentials
2. **Create Slots**: Select date and time slots
3. **Manage System**: Generate 45-minute slots with 6 sub-courts each

## Features in Detail

### OTP Verification System
- 6-digit OTP sent to IIIT email
- 10-minute expiration
- Resend functionality
- Secure verification process

### Smart Slot Management
- **Available**: Green - Ready for booking
- **Partial**: Yellow - Some courts occupied
- **Full**: Red - All courts booked
- Game mode locking on first booking

### Responsive Design
- Mobile-first approach
- Touch-friendly interactions
- Smooth animations on all devices
- Beautiful gradients and shadows

## Development

### Available Scripts
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build

### Customization
- Colors: Modify `tailwind.config.js` primary/secondary colors
- Animations: Adjust Framer Motion transitions
- Components: Extend with new features

## Backend Integration

The frontend connects to the backend API endpoints:
- `/api/auth/*` - Authentication and OTP
- `/api/slots` - Slot management
- `/api/bookings` - Booking operations

Make sure the backend is running on the URL specified in `.env.local`.

## Deployment

### Vercel (Recommended)
1. Push to GitHub
2. Connect repository to Vercel
3. Set environment variables
4. Deploy automatically

### Environment Variables for Production
```env
VITE_API_URL=https://your-backend-url.com
```

## Support

For issues or questions:
1. Check the backend is running
2. Verify environment variables
3. Check browser console for errors
4. Ensure MongoDB connection is active

---

Built with ❤️ for IIIT students
