# ECATS Timesheet Calculator

A modern, professional Progressive Web App (PWA) for accurate timesheet calculations with decimal time conversion, designed specifically for ECATS (Electronic Contractor Time Accounting System) and similar time tracking systems.

## 🚀 Features

- **Sophisticated App Shell Design**: Modern sidebar navigation with integrated calendar
- **Real-time Calculations**: Live updates as you enter time data
- **ECATS Decimal Conversion**: Accurate conversion to decimal hours for time tracking systems
- **Overnight Shifts Support**: Handles shifts that cross midnight
- **Break Time Deduction**: Automatic calculation of net work time after breaks  
- **Late Arrival Tracking**: Identifies and calculates late arrival minutes
- **Progressive Web App**: Install as desktop application, works offline
- **Dark/Light Mode**: Professional themes that adapt to system preferences
- **Export Functionality**: Easy copy-to-clipboard for ECATS entry
- **Quick Actions**: One-click options for today, this week, and timesheet reset

## 📋 Usage Instructions

### Getting Started
1. **Select Work Date**: Use the calendar in the left sidebar to choose your work date
2. **Set Schedule**: Enter your scheduled start and end times (default: 9:00 AM - 5:00 PM)
3. **Record Actual Times**: Enter when you actually started and finished work
4. **Break Time**: Adjust break minutes if different from the 30-minute default
5. **View Results**: The right panel shows live calculations including:
   - Late status and minutes
   - Total work time
   - Net time (after breaks)
   - **ECATS decimal value** for system entry

### Quick Actions (Sidebar)
- **Today**: Jump to today's date
- **This Week**: Navigate to the start of current week
- **Reset Times**: Clear all actual times to start a new entry

### Main Controls (Header)
- **Reset**: Clear timesheet to start fresh
- **Export**: Copy ECATS decimal value to clipboard
- **Theme Toggle**: Switch between light and dark modes
- **Sidebar Toggle**: Collapse/expand the navigation sidebar

### Advanced Tools
Expand the "Advanced Tools" section for:
- **Quick Time Entry**: Set actual end time based on hours and minutes worked
- **Overnight Shift Support**: Automatic handling of shifts crossing midnight
- **Precise Calculations**: All times calculated to the exact minute

## 💻 Installation & Desktop Use

### Desktop Installation (Recommended)
1. Open the application in Chrome, Edge, or Safari
2. Look for the "Install" icon in the address bar
3. Click to install as a desktop application
4. Launch from your desktop or start menu

### Browser Use
- Works in any modern web browser
- Automatically saves your data locally
- No internet connection required after initial load

## 🏗️ Technical Architecture

### Frontend
- **React 18** with TypeScript for type safety
- **Vite** for fast development and optimized builds
- **shadcn/ui** component library built on Radix UI
- **Tailwind CSS** with custom design system
- **Progressive Web App** with service worker for offline functionality

### Design System
- Professional Material Design-inspired interface
- Responsive layout that adapts to all screen sizes
- Sophisticated app shell with sidebar navigation
- Consistent spacing and typography throughout

### Data Management
- Local storage for persistent timesheet data
- No server required - fully client-side application
- Automatic saving with debounced writes
- Form validation with React Hook Form and Zod schemas

## 📁 Project Structure

```
client/src/
├── components/
│   ├── ui/                    # shadcn/ui components
│   ├── MinimalTimesheetCalculator.tsx  # Main calculator logic
│   ├── AppSidebar.tsx        # Navigation sidebar
│   └── ThemeToggle.tsx       # Dark/light mode toggle
├── lib/                      # Utility functions
├── pages/                    # Route components (future expansion)
└── main.tsx                  # Application entry point
```

## 🚀 Deployment Options

### Replit Publishing
1. Click the "Publish" button in Replit
2. Your app will be available at `your-repl-name.replit.app`
3. Custom domains can be configured in Replit settings

### Static Hosting (Netlify, Vercel, GitHub Pages)
1. Run `npm run build` to create production build
2. Deploy the `dist/` folder to your hosting provider
3. Configure for single-page application routing

### Desktop Distribution
1. Install as PWA for local desktop use
2. Use Electron wrapper for native app distribution
3. Package with tools like `electron-builder` for installers

## 📝 Credits & Acknowledgments

### Original Development
**Developer**: A. Ace Sirleaf  
**Copy**: Kola Labs

### Technology Stack
- **React Team** - React framework and ecosystem
- **Vite Team** - Build tool and development server
- **shadcn** - UI component system and design patterns
- **Radix UI** - Accessible component primitives
- **Tailwind CSS** - Utility-first styling framework
- **Lucide** - Beautiful, consistent icons

### Design Inspiration
- **Material Design** - Google's design system principles
- **Apple Human Interface Guidelines** - macOS app design patterns
- **Modern PWA Standards** - Progressive Web App best practices

### Development Tools
- **TypeScript** - Type safety and developer experience
- **ESLint & Prettier** - Code quality and formatting
- **React Hook Form** - Form validation and management
- **Zod** - Runtime type validation

### Special Thanks
Built with modern web standards and accessibility in mind. Designed for contractors and professionals who need accurate, reliable timesheet calculations for various time tracking systems.

---

## 🛠️ Development

### Prerequisites
- Node.js 18 or higher
- npm or yarn package manager

### Local Development
```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

### Contributing
This is a professional timesheet calculator designed for accuracy and ease of use. Contributions should maintain the professional appearance and calculation precision.

---

**Version**: 1.0.0  
**License**: MIT  

For support or feature requests, please refer to your Replit project documentation.

*Built for accurate timesheet calculations with a focus on simplicity and reliability.*