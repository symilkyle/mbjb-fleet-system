# 🚗 MBJB Fleet Tracking System - Prototype

> **Sistem Pengurusan Armada Kenderaan untuk Majlis Bandaraya Johor Bahru**
> 
> Modern fleet management system prototype built with React, featuring real-time GPS tracking, booking management, and driver mobile interface.

[![Live Demo](https://img.shields.io/badge/demo-online-brightgreen)](https://your-github-username.github.io/mbjb-fleet-system/)
[![React](https://img.shields.io/badge/React-18.3.1-blue)](https://reactjs.org/)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

---

## 🌟 Live Demo

**🔗 [View Live Prototype](https://your-github-username.github.io/mbjb-fleet-system/)**

*(Replace with your actual GitHub Pages URL after deployment)*

---

## 📸 Screenshots

### Admin Dashboard
Real-time fleet overview with interactive map and statistics
![Dashboard Preview](https://via.placeholder.com/800x450/1E3A8A/FFFFFF?text=Admin+Dashboard)

### Live Tracking
GPS tracking with vehicle filtering and status monitoring
![Tracking Preview](https://via.placeholder.com/800x450/3B82F6/FFFFFF?text=Live+Tracking)

### Bookings Management
Comprehensive booking request management system
![Bookings Preview](https://via.placeholder.com/800x450/7C3AED/FFFFFF?text=Bookings+Management)

### Driver Mobile Interface
Mobile-optimized interface for drivers
![Driver Preview](https://via.placeholder.com/400x800/10B981/FFFFFF?text=Driver+Interface)

---

## ✨ Features

### 🖥️ Admin Web Dashboard
- **Real-time Fleet Statistics** - Live monitoring of all vehicles
- **Interactive Map** - Leaflet-powered GPS tracking with 10 vehicles
- **Active Alerts Panel** - Real-time notifications for violations
- **Recent Activities Feed** - Comprehensive activity logs
- **Vehicle Filtering** - Filter by status (Moving/Idle/Stopped/Offline)

### 📋 Bookings Management
- **View All Bookings** - 7 sample bookings with different statuses
- **Status Filtering** - Pending (2), Approved (3), Completed (2)
- **Approval Workflow** - Quick approve/reject interface
- **Detailed Information** - Staff, department, destination, purpose

### 📱 Driver Mobile Interface
- **Vehicle Status** - Current vehicle metrics and status
- **Task Management** - Today's task list with priorities
- **Active Trip Tracking** - Live trip monitoring with map
- **Quick Actions** - Refuel, report issues, view history
- **Vehicle Controls** - Start engine, beep sound

### 🎨 Design Highlights
- **Responsive Design** - Optimized for desktop and mobile
- **Modern UI/UX** - Professional blue/purple color scheme
- **Interactive Components** - Maps, filters, status indicators
- **Smooth Animations** - Polished user experience

---

## 🛠️ Technology Stack

| Category | Technology | Version | Purpose |
|----------|-----------|---------|---------|
| **Frontend** | React | 18.3.1 | UI Framework |
| **Build Tool** | Vite | 5.4.21 | Fast development & build |
| **Styling** | Tailwind CSS | 3.4.15 | Utility-first CSS |
| **Routing** | React Router | 7.0.2 | Navigation (Hash-based) |
| **Maps** | Leaflet | 1.9.4 | Interactive mapping |
| **Icons** | Lucide React | 0.469.0 | Modern icon library |
| **Date Utils** | date-fns | 4.1.0 | Date formatting |

---

## 📁 Project Structure

```
mbjb-fleet-system/
├── assets/
│   ├── index-*.css          # Compiled Tailwind CSS
│   └── index-*.js           # Compiled React app
├── index.html               # Main HTML entry point
├── README.md                # This file
└── TEST_PAGE.html           # Local testing guide
```

---

## 🚀 Quick Start

### Option 1: View Online (Recommended)
Simply visit the [Live Demo](https://your-github-username.github.io/mbjb-fleet-system/)

### Option 2: Run Locally

**Method A: Python HTTP Server** (Easiest)
```bash
# Navigate to project folder
cd mbjb-fleet-system

# Start server
python -m http.server 8000

# Open browser
http://localhost:8000
```

**Method B: Node.js HTTP Server**
```bash
# Install http-server globally
npm install -g http-server

# Navigate to project folder
cd mbjb-fleet-system

# Start server
http-server -p 8000

# Open browser
http://localhost:8000
```

**Method C: VS Code Live Server**
1. Open folder in VS Code
2. Right-click `index.html`
3. Select "Open with Live Server"

---

## 🧭 Navigation Guide

### Admin Routes (Desktop)
- **Dashboard:** `#/admin` (default)
- **Live Tracking:** `#/admin/tracking`
- **Bookings:** `#/admin/bookings`
- **Other Pages:** Under construction placeholders

### Driver Routes (Mobile)
- **Driver Home:** `#/driver`
- **Active Trip:** `#/driver/trip`

**Note:** URLs use hash routing (`#/`) for offline compatibility.

---

## 📊 Mock Data

The prototype includes realistic mock data:
- **10 Vehicles** - Various brands and statuses
- **7 Bookings** - Pending, approved, and completed requests
- **5 Active Alerts** - Different severity levels
- **Recent Activities** - System logs and events
- **Trip History** - Sample trip data

---

## 🎯 Key Components

### StatCard
Dashboard statistics with icons, values, and trend indicators
- Color-coded by status (green/red/yellow/gray)
- Animated on load

### MapView
Interactive Leaflet map integration
- Custom markers by vehicle status
- Popup details on click
- Auto-center to Johor Bahru

### VehicleCard
Comprehensive vehicle information display
- Status indicators
- Driver details
- Metrics (speed, fuel, battery)

### BookingCard
Booking request cards with detailed information
- Timeline display
- Status badges
- Approval actions

---

## 🎨 Design System

### Color Palette
| Color | Hex Code | Usage |
|-------|----------|-------|
| Primary Blue | `#1E3A8A` → `#3B82F6` | Headers, buttons, nav |
| Purple Accent | `#7C3AED` → `#A78BFA` | Highlights, badges |
| Success Green | `#10B981` | Moving status |
| Warning Orange | `#F59E0B` | Idle status |
| Danger Red | `#EF4444` | Alerts, stopped |
| Neutral Gray | `#6B7280` → `#F9FAFB` | Text, backgrounds |

### Typography
- **Headers:** Helvetica Bold, 24-32px
- **Body:** Helvetica Regular, 14-16px
- **Labels:** Helvetica Medium, 12-14px

---

## ⚠️ Limitations

This is a **prototype** with the following limitations:
- ❌ Mock/hardcoded data (no database)
- ❌ Simulated tracking (no real GPS)
- ❌ No backend API
- ❌ No authentication
- ❌ Changes not persisted

**Purpose:** Demonstration and evaluation only

---

## 🚀 Future Development Roadmap

### Phase 1: Backend Integration (2-3 months)
- [ ] REST API development (Node.js/Laravel)
- [ ] PostgreSQL/MySQL database
- [ ] Real-time WebSocket for live updates
- [ ] JWT authentication & authorization
- [ ] GPS device integration

### Phase 2: Feature Completion (1-2 months)
- [ ] Vehicle management module
- [ ] Reports generation system
- [ ] Maintenance tracking
- [ ] Advanced analytics with charts
- [ ] Staff booking form
- [ ] Push notifications

### Phase 3: Advanced Features (2-3 months)
- [ ] Real GPS tracking from devices
- [ ] Route optimization algorithms
- [ ] Geofencing and automated alerts
- [ ] File uploads (photos, documents)
- [ ] Export reports (PDF, Excel)
- [ ] Advanced analytics dashboard

### Phase 4: Mobile Applications (3-4 months)
- [ ] React Native iOS app
- [ ] React Native Android app
- [ ] Offline mode support
- [ ] Native GPS integration
- [ ] Camera integration
- [ ] App Store deployment

### Phase 5: Testing & Deployment (1-2 months)
- [ ] User acceptance testing
- [ ] Performance optimization
- [ ] Security audits
- [ ] Load testing
- [ ] Production deployment
- [ ] User training & documentation

**Total Estimated Timeline:** 9-14 months for complete system

---

## 💻 Development

### Prerequisites
- Node.js 18+
- npm or yarn

### Build from Source
```bash
# Clone repository
git clone https://github.com/your-username/mbjb-fleet-system.git
cd mbjb-fleet-system

# Install dependencies
npm install

# Run development server
npm run dev

# Build for production
npm run build
```

### Configuration
For GitHub Pages deployment, ensure `base: './'` in `vite.config.js` for relative paths.

---

## 📱 Responsive Design

The application is fully responsive:
- **Desktop (>1024px):** Full admin panel with sidebar
- **Tablet (768-1024px):** Collapsible sidebar, adjusted layouts
- **Mobile (<768px):** Bottom navigation, stacked components

---

## 🤝 Contributing

This is a prototype project for MBJB. For production development:
1. Fork the repository
2. Create feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open Pull Request

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Developer

**Built for:** Majlis Bandaraya Johor Bahru (MBJB)  
**Version:** Prototype 2.0  
**Build Date:** November 2025  

---

## 📞 Support

For questions or issues:
- Open an issue on GitHub
- Contact: [your-email@example.com]

---

## 🙏 Acknowledgments

- **OpenStreetMap** - Map tiles provider
- **Leaflet** - Mapping library
- **React Team** - Framework
- **Tailwind Labs** - CSS framework
- **Lucide** - Icon library

---

<div align="center">

### ⭐ Star this repo if you find it helpful!

**Made with ❤️ for MBJB Fleet Management**

[View Demo](https://your-github-username.github.io/mbjb-fleet-system/) • [Report Bug](https://github.com/your-username/mbjb-fleet-system/issues) • [Request Feature](https://github.com/your-username/mbjb-fleet-system/issues)

</div>
