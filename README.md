# 🍕 Jab We Ate - Fast React Pizza

A modern, fast pizza ordering application built with React, Redux Toolkit, and React Router. Order your favorite pizzas with a seamless user experience and real-time order tracking.

## ✨ Features

### 🛒 Shopping Experience
- **Browse Menu**: View a complete pizza menu with prices and ingredients
- **Smart Cart Management**: Add, remove, and update pizza quantities in your cart
- **Real-time Cart Updates**: See your cart total update instantly as you modify items
- **Priority Orders**: Option to mark orders as priority for faster delivery

### 👤 User Features
- **Personalized Experience**: Enter your name to get a customized ordering experience
- **Order Tracking**: Search and track your orders by order ID
- **Geolocation Support**: Automatically fetch your address using geolocation API
- **Order History**: View detailed order information including items, prices, and delivery status

### 🎨 User Interface
- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Modern UI**: Built with Tailwind CSS for a clean, professional look
- **Loading States**: Smooth loading indicators for better UX
- **Error Handling**: Comprehensive error pages and user-friendly error messages

## 🛠️ Tech Stack

### Frontend
- **React 18.2** - Modern React with hooks
- **React Router DOM 6.30** - Client-side routing with loaders and actions
- **Redux Toolkit 2.9** - State management
- **React Redux 9.2** - React bindings for Redux

### Styling
- **Tailwind CSS 3.4** - Utility-first CSS framework
- **PostCSS** - CSS processing
- **Roboto Mono** - Google Fonts integration

### Build Tools
- **Vite 4.4** - Fast build tool and dev server
- **ESLint** - Code linting
- **Prettier** - Code formatting with Tailwind plugin

### Deployment
- **Netlify** - Configured for seamless deployment with SPA routing

## 📦 Installation

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn

### Setup

1. **Clone the repository**
```bash
git clone <repository-url>
cd 16-fast-react-pizza
```

2. **Install dependencies**
```bash
npm install
```

3. **Start development server**
```bash
npm run dev
```

4. **Open your browser**
Navigate to `http://localhost:5173` (or the port shown in your terminal)

## 🚀 Available Scripts

- `npm run dev` - Start development server with hot reload
- `npm run build` - Build production-ready bundle
- `npm run preview` - Preview production build locally
- `npm run lint` - Run ESLint to check code quality

## 📁 Project Structure

```
16-fast-react-pizza/
├── public/              # Static assets
├── src/
│   ├── features/        # Feature-based modules
│   │   ├── cart/        # Shopping cart functionality
│   │   │   ├── Cart.jsx
│   │   │   ├── CartItem.jsx
│   │   │   ├── CartOverview.jsx
│   │   │   ├── DeleteItem.jsx
│   │   │   ├── EmptyCart.jsx
│   │   │   ├── UpdateItemQuantity.jsx
│   │   │   └── cartSlice.js
│   │   ├── menu/        # Pizza menu display
│   │   │   ├── Menu.jsx
│   │   │   └── MenuItem.jsx
│   │   ├── order/       # Order creation and tracking
│   │   │   ├── CreateOrder.jsx
│   │   │   ├── Order.jsx
│   │   │   ├── OrderItem.jsx
│   │   │   ├── SearchOrder.jsx
│   │   │   └── UpdateOrder.jsx
│   │   └── user/        # User management
│   │       ├── CreateUser.jsx
│   │       ├── Username.jsx
│   │       └── userSlice.js
│   ├── services/        # API services
│   │   ├── apiGeocoding.js
│   │   └── apiRestaurant.js
│   ├── ui/              # Reusable UI components
│   │   ├── AppLayout.jsx
│   │   ├── Button.jsx
│   │   ├── Error.jsx
│   │   ├── Header.jsx
│   │   ├── Home.jsx
│   │   ├── LinkButton.jsx
│   │   └── Loader.jsx
│   ├── utils/           # Utility functions
│   ├── App.jsx          # Main app component with routing
│   ├── index.css        # Global styles
│   ├── main.jsx         # App entry point
│   └── store.js         # Redux store configuration
├── index.html           # HTML template
├── netlify.toml         # Netlify deployment config
├── package.json         # Dependencies and scripts
├── tailwind.config.js   # Tailwind configuration
├── vite.config.js       # Vite configuration
└── README.md            # This file
```

## 🏗️ Architecture

### State Management
The application uses **Redux Toolkit** for state management with two main slices:
- **User Slice**: Manages user information (username)
- **Cart Slice**: Manages shopping cart state (items, quantities, totals)

### Routing
**React Router v6** is used with the following routes:
- `/` - Home page with user creation
- `/menu` - Browse pizza menu
- `/cart` - View and manage cart
- `/order/new` - Create new order
- `/order/:orderId` - View specific order details

### Data Fetching
- Uses React Router's `loader` functions for data fetching
- Uses React Router's `action` functions for form submissions
- API services handle external API calls (restaurant menu, geocoding)

## 🌐 Deployment

The application is configured for deployment on **Netlify**:

1. **Build the project**
```bash
npm run build
```

2. **Deploy to Netlify**
- Connect your repository to Netlify
- Set build command: `npm run build`
- Set publish directory: `dist`
- The `netlify.toml` file handles SPA routing automatically

## 🎯 Key Features Implementation

### Cart Management
- Add/remove items with smooth animations
- Update quantities directly from cart
- Persistent cart state using Redux
- Real-time price calculations

### Order System
- Form validation for order creation
- Priority order option with additional cost
- Order tracking by ID
- Geolocation integration for address

### Responsive Design
- Mobile-first approach
- Tailwind CSS breakpoints for different screen sizes
- Touch-friendly interface for mobile devices

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📝 License

This project is part of an internship learning exercise.

## 🙏 Acknowledgments

- Pizza menu data from external API
- Geocoding services for address lookup
- Modern React patterns and best practices

---

**Built with ❤️ using React and Vite**
