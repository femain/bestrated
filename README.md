# Best Rated Hospitals - Healthcare Web Application

A modern, responsive healthcare web application for finding and rating hospitals. Features integrated branding with logo and background assets, mobile-optimized design, and automated deployment capabilities.

## 🚀 Deployment

This project includes automated FTP deployment via GitHub Actions. Every push to the `main` branch will automatically deploy to your FTP server.

### Setting up FTP Deployment

1. **Configure Repository Secrets** in your GitHub repository settings:
   - `FTP_USERNAME`: Your FTP username
   - `FTP_PASSWORD`: Your FTP password

2. **Update FTP Settings** in `.github/workflows/deploy.yml`:
   - Replace `ftp.yourdomain.com` with your FTP server
   - Adjust `server-dir` to match your hosting directory (e.g., `/public_html/`)

3. **Push to Main Branch**: Deployment happens automatically on every push to `main`

## 📁 File Structure

```
html-pages/
├── styles.css              # Main stylesheet with all styling
├── index.html              # Homepage with hero section and features
├── login.html              # User authentication page
├── register.html           # Patient registration form
├── register-hospital.html  # Hospital registration form
├── search.html             # Hospital search and listing page
├── hospital.html           # Individual hospital details page
├── review.html             # Hospital rating/review form
├── reset-password.html     # Password reset page
└── README.md              # This documentation file
```

## 🚀 Getting Started

1. **Open any HTML file** in your web browser
2. **Start with `index.html`** for the homepage experience
3. **Navigate between pages** using the navigation links or buttons

No server setup or build process required - these are pure HTML/CSS/JavaScript files.

## 📄 Page Descriptions

### 🏠 Landing Page (`index.html`)
- **Purpose**: Homepage showcasing the application's features
- **Features**:
  - Hero section with parallax background
  - Four feature cards explaining the platform
  - Registration call-to-action section
  - Sample hospital rankings display
- **Navigation**: Links to all other pages

### 🔐 Login Page (`login.html`)
- **Purpose**: User authentication interface
- **Features**:
  - Username/email and password fields
  - Form validation
  - Links to registration and password reset
- **Functionality**: Simulated login process (alerts for demo)

### 👤 Register Page (`register.html`)
- **Purpose**: Patient account creation
- **Features**:
  - Username, email, and password fields
  - Client-side validation (length, email format)
  - Link to login page
- **Validation**: Real-time form validation with user feedback

### 🏥 Hospital Registration (`register-hospital.html`)
- **Purpose**: Hospital account creation
- **Features**:
  - Comprehensive hospital information form
  - Dynamic state/region selection
  - Description field with character limit
  - Full form validation
- **Data**: Includes Nigerian states and regions

### 🔍 Search Page (`search.html`)
- **Purpose**: Hospital discovery and filtering
- **Features**:
  - Search by name or location
  - State-based filtering
  - Interactive hospital cards with ratings
  - Live search functionality
- **Sample Data**: 4 sample hospitals with realistic information

### 🏥 Hospital Details (`hospital.html`)
- **Purpose**: Detailed hospital information and actions
- **Features**:
  - Hospital contact information and verification status
  - Quality profile with multiple score metrics
  - Interactive dialogs for reports and profile editing
  - Location map placeholder
  - Links to rating system
- **Interactions**: Modal dialogs for downloads and editing

### ⭐ Review Page (`review.html`)
- **Purpose**: Hospital rating and feedback system
- **Features**:
  - Visit information form (date, diagnosis, length of stay)
  - Multi-category question system with tabs
  - 4-point Likert scale ratings
  - Form completion validation
  - Dynamic submit button activation
- **Categories**: Patient Safety, Quality Management, Communication

### 🔑 Reset Password (`reset-password.html`)
- **Purpose**: Password recovery interface
- **Features**:
  - Email input with validation
  - Simple, clean interface
  - Link back to login page

## 🎨 Styling and Design

### Color Scheme
- **Primary**: `#4392f1` (Blue)
- **Alternate**: `#53d8fb` (Light Blue)
- **Secondary**: `#363732` (Dark Gray)
- **Accent Colors**: Yellow (`#ffeb3b`), Success (`#4caf50`), Orange (`#ff9800`), Red (`#f44336`)

### Typography
- **Body Text**: 'Nunito Sans', sans-serif
- **Headings**: 'Open Sans', sans-serif (bold)
- **Icons**: Material Icons font

### Layout System
- **Responsive Grid**: Custom flexbox-based grid system
- **Breakpoints**: Mobile-first responsive design
- **Components**: Cards, buttons, forms, dialogs, tabs

### Key Features
- **Material Design Inspired**: Clean, modern interface
- **Responsive Design**: Works on desktop, tablet, and mobile
- **Interactive Elements**: Hover effects, transitions, animations
- **Accessibility**: Proper form labels, semantic HTML structure

## 🔧 Interactive Features

### Form Validation
- Real-time validation feedback
- Email format checking
- Password strength requirements
- Required field validation
- Character limits and constraints

### Dynamic Content
- **State/Region Selection**: Cascading dropdowns in hospital registration
- **Tab Navigation**: Multi-category question system in reviews
- **Search Filtering**: Live hospital filtering on search page
- **Modal Dialogs**: Report downloads and profile editing

### Navigation
- **Consistent Header**: Navigation bar on all pages
- **Breadcrumb Links**: Hospital name links back to details
- **Call-to-Action Buttons**: Strategic placement throughout

## 📱 Responsive Design

### Mobile Optimization
- **Flexible Grid**: Columns stack on smaller screens
- **Touch-Friendly**: Appropriately sized buttons and form elements
- **Readable Text**: Optimized font sizes and spacing
- **Navigation**: Mobile-friendly menu system

### Desktop Experience
- **Multi-Column Layouts**: Efficient use of screen real estate
- **Hover Effects**: Enhanced interactivity
- **Larger Content Areas**: Comfortable reading and interaction

## 🔄 Simulated Functionality

Since these are static HTML pages, the following features are simulated:

### Authentication
- Login attempts show success/error alerts
- Registration processes display confirmation messages
- Password reset sends simulated email notifications

### Data Management
- Hospital search filters existing sample data
- Form submissions log data to browser console
- Profile updates show success confirmations

### File Operations
- Report downloads trigger browser alerts
- Payment processes show integration placeholders
- Map displays show placeholder content

## 🚀 Deployment Options

### Static Hosting
- **GitHub Pages**: Upload to repository and enable Pages
- **Netlify**: Drag and drop the folder for instant deployment
- **Vercel**: Connect repository for automatic deployments
- **AWS S3**: Upload files to S3 bucket with static website hosting

### Local Development
- **Live Server**: Use VS Code Live Server extension
- **Python**: `python -m http.server 8000`
- **Node.js**: `npx serve .`
- **Direct File**: Open HTML files directly in browser

## 🔮 Future Enhancements

### Backend Integration
- Connect forms to actual API endpoints
- Implement real user authentication
- Add database connectivity for hospital data
- Integrate payment processing

### Advanced Features
- **Real Maps**: Google Maps or Mapbox integration
- **Image Uploads**: Hospital photos and user avatars
- **Advanced Search**: Filters by specialties, ratings, distance
- **Reviews System**: User-generated reviews and ratings
- **Notifications**: Email and in-app notifications

### Performance Optimizations
- **Image Optimization**: WebP format, lazy loading
- **CSS/JS Minification**: Reduce file sizes
- **Caching Strategies**: Browser and CDN caching
- **Progressive Web App**: Offline functionality, app-like experience

## 🛠️ Customization Guide

### Styling Changes
- **Colors**: Update CSS custom properties in `:root`
- **Fonts**: Change font imports and font-family declarations
- **Layout**: Modify grid classes and responsive breakpoints

### Content Updates
- **Hospital Data**: Update sample hospitals in search.html
- **Questions**: Modify review questions in review.html
- **States/Regions**: Update location data in register-hospital.html

### Feature Additions
- **New Pages**: Follow existing page structure and styling patterns
- **Form Fields**: Use existing form classes and validation patterns
- **Interactive Elements**: Follow modal and tab implementation examples

## 📞 Support and Documentation

### Browser Compatibility
- **Modern Browsers**: Chrome, Firefox, Safari, Edge (latest versions)
- **Mobile Browsers**: iOS Safari, Chrome Mobile, Samsung Internet
- **Fallbacks**: Graceful degradation for older browsers

### Accessibility
- **Semantic HTML**: Proper heading hierarchy and landmarks
- **Form Labels**: Associated labels for all form inputs
- **Keyboard Navigation**: Tab order and focus management
- **Screen Readers**: ARIA labels where appropriate

---

**Note**: This HTML version provides a complete user interface experience for the Best Rated Hospitals application. While the backend functionality is simulated, the interface is fully functional and ready for integration with a real backend system.
