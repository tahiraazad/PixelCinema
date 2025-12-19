# 🎬PixelCinema - Online Movie Ticket Reservation System

> A modern, fully-functional movie ticket booking web application built with vanilla HTML, CSS, and JavaScript featuring real-time seat selection, AJAX integration, and QR code generation.

<p align="center">
<a href="https://www.w3schools.com/html/" target="_blank" rel="noreferrer"> <img src="https://skillicons.dev/icons?i=html" alt="html" width="70" height="70"/> </a> 
<a href="#" target="_blank" rel="noreferrer"> <img src="https://skillicons.dev/icons?i=css" alt="css" width="70" height="70"/> </a>
<a href="#" target="_blank" rel="noreferrer"> <img src="https://skillicons.dev/icons?i=js" alt="javascript" width="70" height="70"/> </a>

</p>

## 🌟 Overview

PixelCinema is a premium online movie ticket reservation platform designed for Sri Lankan cinema-goers. This Single Page Application (SPA) provides an intuitive and seamless booking experience with real-time seat availability, interactive seat selection, and instant ticket confirmation with QR codes.

### Why PixelCinema?

- **Real-Time Updates**: AJAX-powered seat availability checking
- **Modern UI/UX**: Glassmorphic navigation with smooth animations
- **Mobile-First**: Fully responsive design for all devices
- **Secure**: Client-side validation with error handling
- **Local Currency**: All transactions in LKR (Sri Lankan Rupees)

## ✨ Features

### 🎯 Core Features

- **Hero Slider**: Auto-rotating image carousel with manual navigation
- **Movie Catalog**: Browse 8+ movies with detailed information
- **Real-Time Seat Selection**: Interactive cinema hall with 96 seats (8 rows × 12 seats)
- **Live Seat Status**: 
  - Available (clickable)
  - Selected (user's choice)
  - Occupied (pre-booked via AJAX)
- **Smart Form Validation**: 
  - Real-time input validation
  - Email format checking (regex)
  - Phone number validation
  - Dynamic button enabling/disabling
- **QR Code Generation**: Unique QR codes for each booking
- **Ticket Download**: Export booking confirmation
- **Search Functionality**: Real-time movie search

### 🎨 UI/UX Features

- **Glassmorphic Navigation Bar**: 
  - Fixed position with blur effects
  - Scroll-triggered style changes
  - Mobile-responsive hamburger menu
- **Dark Cinema Theme**: Immersive viewing experience
- **Smooth Animations**: Fade-ins, scale effects, hover transitions
- **Loading Indicators**: Visual feedback during AJAX calls
- **Responsive Design**: Optimized for mobile, tablet, and desktop

### 🔧 Technical Features

- **AJAX Integration**: Asynchronous seat availability fetching
- **JSON Data Handling**: Structured data management
- **Local Storage**: Session state management
- **Error Handling**: Graceful fallbacks for images and data
- **Cross-Browser Compatible**: Works on modern browsers


## 🎥 Demo

### Live Demo

[View Live Demo](https://darkfeed2005.github.io/PixelCinema/)



## 🛠️ Technologies Used

### Frontend
- **HTML5**: Semantic markup structure
- **CSS3**: 
  - Flexbox & Grid layouts
  - CSS Custom Properties (Variables)
  - Glassmorphism effects
  - Responsive media queries
- **JavaScript (ES6+)**:
  - Async/Await for AJAX
  - DOM manipulation
  - Event handling
  - Form validation with regex

### Libraries & APIs
- **QRCode.js**: QR code generation
- **CDN**: CloudFlare for external libraries

### Design Patterns
- Single Page Application (SPA)
- State Management
- Component-Based Structure
- Event-Driven Architecture

## 📦 Installation

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/DarkFeed2005/PixelCinema.git
   cd PixelCinema
   ```

2. **Run the application**
   ```bash
   # Simply open index.html in your browser
   open index.html
   ```
   

## 🚀 Usage

### Booking a Ticket

1. **Browse Movies**: 
   - Navigate to the home page
   - View featured movies in the hero slider
   - Scroll down to see the full movie catalog

2. **Select Movie & Showtime**:
   - Choose your preferred movie
   - Select a showtime from the dropdown
   - Click "Select This Movie"

3. **Choose Seats**:
   - AJAX loads real-time seat availability
   - Click on available (gray) seats to select them
   - Selected seats turn blue
   - View live price updates in the summary

4. **Fill Customer Details**:
   - Enter your full name
   - Provide a valid email address
   - Add your phone number
   - Form validates in real-time

5. **Complete Booking**:
   - Click "Book Now" (enabled after validation)
   - View confirmation with booking details
   - Scan/save QR code for entry
   - Download ticket as needed

### Search Feature
- Use the search bar in navigation
- Type movie name to filter results
- Results update in real-time

## 📁 Project Structure

```
PixelCinema/
│
├── index.html              # Main HTML file (includes CSS & JS)
│
├── assets/                 # Movie poster images
│   ├── Avatar_Fire_and_As.jpg
│   ├── Black_Phone_2_post.jpg
│   ├── F1_(2025_film).png
│   ├── Love_Aaj_Kal_film_p.jpg
│   ├── Neera_film_poster.jpg
│   ├── Sisu_ver2.png
│   ├── The_Conjuring_-_La.jpg
│   └── Zootopia_2_(2025_film).jpg
│
│
└── README.md              # Project documentation
```

### Code Structure

The application is built as a single HTML file with embedded CSS and JavaScript:

- **CSS Section**: Complete styling with CSS custom properties
- **JavaScript Section**:
  - Data layer (movie database, configuration)
  - State management
  - AJAX functions
  - Utility functions
  - Rendering functions
  - Event handlers
  - Initialization code

## 🔌 API Integration

### AJAX Seat Availability

The application simulates real-time seat availability checking using AJAX:

```javascript
// Simulated API call
async function fetchSeatAvailability(movieId, showtime) {
    // Shows loading indicator
    // Simulates 500-1500ms API delay
    // Returns JSON with occupied seat data
}
```

### JSON Response Format

```json
{
  "success": true,
  "movieId": 1,
  "showtime": "2:00 PM",
  "totalSeats": 96,
  "occupiedSeats": [
    {"row": 0, "seat": 3},
    {"row": 2, "seat": 7},
    ...
  ],
  "timestamp": "2024-12-19T10:30:00.000Z"
}
```

### Backend Integration (Future)

To connect with a real backend:

1. Replace `fetchSeatAvailability()` with actual API endpoint
2. Update JSON structure to match your backend
3. Add authentication tokens if required
4. Implement proper error handling

## 🔮 Future Enhancements

### Planned Features

- [ ] **User Authentication**: Login/Register system
- [ ] **Payment Gateway**: Integrate payment processing
- [ ] **Email Notifications**: Send booking confirmations
- [ ] **Admin Dashboard**: Manage movies and bookings
- [ ] **Multi-Cinema Support**: Choose different theaters
- [ ] **Seat Pricing Tiers**: Premium, standard, economy seats
- [ ] **Food & Beverage**: Add concession ordering
- [ ] **Loyalty Program**: Rewards and discounts
- [ ] **Social Sharing**: Share movie plans on social media
- [ ] **Review & Ratings**: User reviews for movies
- [ ] **Backend API**: Complete REST API integration
- [ ] **Database**: MySQL/MongoDB for data persistence
- [ ] **PDF Tickets**: Generate downloadable PDF tickets
- [ ] **Multi-Language**: Support Sinhala, Tamil, English

### Technical Improvements

- [ ] Progressive Web App (PWA)
- [ ] Service Workers for offline mode
- [ ] Performance optimization
- [ ] Accessibility (WCAG) compliance
- [ ] Unit testing with Jest
- [ ] E2E testing with Cypress
- [ ] CI/CD pipeline
- [ ] Docker containerization

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

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

👨‍💻 Author
 
- Kalana Yasassri  <a href="https://github.com/DarkFeed2005" target="_blank" rel="noreferrer"> <img src="https://skillicons.dev/icons?i=github" alt="github" width="20" height="20"/> </a>
- LinkedIn <a href="https://www.linkedin.com/in/kalana-yasassri-684591251/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/linkedin/linkedin-original.svg" alt="linkedin" width="20" height="20"/> </a>
- Instagram <a href="https://www.instagram.com/kalana_yasassri/" target="_blank" rel="noreferrer"> <img src="https://skillicons.dev/icons?i=instagram" alt="instagram" width="20" height="20"/> </a> 
  
🎨 License
This project is open-source under the MIT License.


