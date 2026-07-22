# LeadPilot – AI Sales Intelligence Platform

A modern, AI-powered SaaS platform for finding, scoring, and engaging sales prospects with zero friction.

## 📁 Project Structure

```
LeadPilot/
├── index.html              # Landing page & auth (Login, Register)
├── dashboard.html          # Main application dashboard
│
├── css/
│   ├── style.css          # Landing page & global styles (17 KB)
│   └── dashboard.css      # Dashboard & app component styles (35 KB)
│
├── js/
│   ├── app.js             # Landing page logic, navigation, modals (7.4 KB)
│   └── dashboard.js       # Dashboard app, all page controllers (107 KB)
│
└── README.md              # This file
```

## 🚀 Quick Start

### 1. Open Landing Page
```bash
# Open in browser
open index.html
```

**Landing page features:**
- ✅ Hero section with CTA buttons
- ✅ Features showcase (6 sections)
- ✅ Pricing table (3 plans)
- ✅ Testimonials carousel
- ✅ FAQ accordion
- ✅ Language selector (EN, CS, RU)
- ✅ Navigation to Login/Register/Dashboard

### 2. Go to Dashboard
Click **"Start free trial"** button → Opens `dashboard.html`

**Dashboard features:**
- ✅ Sidebar navigation (10 sections)
- ✅ Topbar with search, notifications, language switcher
- ✅ KPI cards with sparklines
- ✅ Charts (Lead Growth, Revenue, Email Performance)
- ✅ Recent Activity feed
- ✅ Fully functional page routing
- ✅ User profile dropdown
- ✅ All interactive elements working

### 3. Demo Credentials
```
Email:    demo@leadpilot.io
Password: demo1234
```

## 📋 Features Implemented

### ✅ Landing Page (`index.html`)
- Responsive navigation bar
- Hero section with statistics
- 6 feature cards
- How-it-works section (3 steps)
- Pricing table with badges
- Customer testimonials
- FAQ accordion (expandable)
- Footer with links
- Language switching (EN/CS/RU)
- Modal system for demos
- Auth pages (Login, Register, Forgot Password)

### ✅ Dashboard (`dashboard.html`)
- Complete HTML5 structure with DOCTYPE
- External CSS linked properly
- Sidebar with navigation (10 pages)
- Topbar with search and actions
- 5 KPI cards with sparklines
- 3 chart containers (SVG rendering)
- Recent activity feed
- User dropdown menu with logout
- Notification center (mock)
- Language selector
- Mobile-responsive sidebar toggle
- All page placeholders ready

### ✅ JavaScript (`js/app.js`)
- `showPage(page)` - Switch between landing pages
- `scrollToSection(id)` - Smooth scroll to section
- `showDemoModal()` - Display demo video modal
- `toggleDropdown(id)` - Dropdown toggle logic
- `setLang(lang)` - Language switching with localStorage
- `toggleFaq(element)` - FAQ accordion
- `goToDashboard()` - Navigate to dashboard
- `goToLogin()` / `goToRegister()` - Navigate to auth pages
- `showToast(message, type)` - Toast notifications

### ✅ JavaScript (`js/dashboard.js`)
- Complete SPA (Single Page Application)
- Page router with hash-based navigation
- Multilingual i18n system (EN/CS/RU)
- localStorage persistence
- **Page Controllers:**
  - Dashboard (Charts, KPI rendering)
  - Leads (CRUD, filtering, pagination, export)
  - AI Search (Lead scoring simulation)
  - Email Generator (Email generation with templates)
  - Campaigns (Create, pause, resume, delete)
  - Analytics (Chart rendering)
  - Integrations (Connect/disconnect services)
  - Billing (Plan selection, payments)
  - Settings (Notifications, workspace, API keys, SMTP)
  - Profile (User info, password change, 2FA)
- **UI Systems:**
  - Modal system with backdrop
  - Toast notifications
  - Dropdown menus
  - Breadcrumbs & pagination
  - Form validation
- **Data Management:**
  - Mock seed data (SEED_LEADS, SEED_CAMPAIGNS)
  - localStorage wrapper (Store module)
  - CSV export functionality
  - File import (drag & drop)

### ✅ Styling (`css/style.css`)
- Modern design system with CSS variables
- Comprehensive component library
- Responsive grid system
- Utility classes (flex, grid, spacing, colors)
- Buttons, inputs, cards, badges, avatars
- Modal & toast animations
- Landing page sections
- Auth pages styling
- Mobile-first responsive design

### ✅ Styling (`css/dashboard.css`)
- Complete dashboard design system
- Sidebar + topbar layout
- KPI cards with hover effects
- Chart styling
- Tables with sorting
- Score badges (A/B/C/D)
- Status badges
- Form styling
- Modal system
- Toast notifications
- Dropdown menus
- Responsive adjustments

## 🔌 Navigation Flow

```
Landing Page (index.html)
    ↓
    ├─ [Start Free Trial] → Dashboard
    ├─ [Watch Demo] → Modal
    ├─ [Log in] → Login Page
    ├─ [Features/Pricing/FAQ] → Smooth scroll
    └─ [Language] → Change language
    
Dashboard (dashboard.html)
    ├─ Sidebar Nav → All 10 pages
    ├─ Leads → Add/Edit/Delete/Export
    ├─ AI Search → Analyze leads
    ├─ Email Gen → Generate personalized emails
    ├─ Campaigns → Create & manage campaigns
    ├─ Analytics → View reports
    ├─ Integrations → Connect services
    ├─ Billing → Manage subscription
    ├─ Settings → Configure app
    ├─ Profile → Edit user info
    └─ [Sign Out] → Back to landing
```

## 📱 Responsive Design

- ✅ Mobile-first approach
- ✅ Breakpoints: 600px, 900px, 1140px
- ✅ Mobile menu toggle (hamburger)
- ✅ Sidebar overlay on mobile
- ✅ Flexible grid layouts
- ✅ Touch-friendly buttons

## 🎨 Design System

### Colors
- **Primary:** `#2563EB` (Blue)
- **Success:** `#10B981` (Green)
- **Error:** `#EF4444` (Red)
- **Warning:** `#F59E0B` (Yellow)
- **Dark:** `#1F2937` (Gray-800)

### Spacing
- Grid: `4px` base unit
- Gaps: `8px`, `12px`, `16px`, `24px`

### Typography
- Font: Inter, -apple-system, BlinkMacSystemFont
- Sizes: 12px, 13px, 14px, 15px, 16px, 20px, 24px, 30px, 36px, 52px

## 📊 Mock Data

### Leads (10 companies)
- TechScale GmbH (Berlin, Germany)
- LogiFlow s.r.o. (Prague, Czech Republic)
- FinVault AG (Zürich, Switzerland)
- CloudBurst Inc (Austin, USA)
- DataSynth Ltd (London, UK)
- MarketEdge (Warsaw, Poland)
- EcoShip BV (Amsterdam, Netherlands)
- GrowthBox SRL (Bucharest, Romania)
- AutoTech Brno (Brno, Czech Republic)
- Rosemann & Co (Munich, Germany)

### Campaigns (4 campaigns)
- Germany SaaS Q1 (active) - 145 leads
- Prague Logistics (paused) - 52 leads
- UK Fintech (draft) - 78 leads
- EU E-commerce Outreach (completed) - 200 leads

### User
- Name: Alex Johnson
- Email: alex@company.com
- Plan: Pro
- Credits: 820 / 1,000

## 🔧 Development

### No Build Required
This is a **vanilla JavaScript** project with **no build tools** needed. Simply open in browser.

### File Size
- `index.html` - ~20 KB
- `dashboard.html` - ~26 KB
- `css/style.css` - ~17 KB
- `css/dashboard.css` - ~35 KB
- `js/app.js` - ~7 KB
- `js/dashboard.js` - ~107 KB
- **Total:** ~212 KB (uncompressed)

### Browser Support
- ✅ Chrome/Edge 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Mobile browsers

## 🔐 Authentication

Currently using **mock authentication** for demo purposes.

### To connect real auth:
```javascript
// Replace in js/dashboard.js:
Auth.logout() → supabase.auth.signOut()
Auth.getUser() → supabase.auth.user()
Auth.updateUser() → supabase.auth.updateUser()
```

## 🌐 API Integration

All API endpoints are marked with `⚡ BACKEND` comments for easy replacement:

### Leads API
```javascript
// Line 19-23 in dashboard.js
api: {
  base: '/api/v1',
  leads: '/api/v1/leads',
  campaigns: '/api/v1/campaigns',
  aiScore: '/api/v1/ai/score',
  aiEmail: '/api/v1/ai/email',
}
```

### Replace Mock Data
- Line 701: `AI.scoreLeadAI()` → Real AI API
- Line 732: `AI.generateEmailAI()` → Real email API
- Line 902: `Store.get('leads')` → API fetch

## 🐛 Browser Console

**Expected on first load:**
```
✅ LeadPilot v1.0.0 loaded.
localStorage keys: lp_leads, lp_campaigns, lp_settings, lp_user, ...
```

**Should NOT see:**
- ❌ Uncaught ReferenceError
- ❌ CSS not loading
- ❌ Navigation not working

## 📝 Internationalization

Supported languages: **English (EN), Čeština (CS), Русский (RU)**

Language storage:
```javascript
localStorage.getItem('lp_lang')  // 'en', 'cs', or 'ru'
```

To add new language, edit `TRANSLATIONS` in `js/app.js` and `js/dashboard.js`.

## 🚀 Next Steps

### Phase 1: Backend Integration
- [ ] Replace mock data with real API
- [ ] Implement authentication (Supabase/Auth0)
- [ ] Connect to database (Supabase/PostgreSQL)

### Phase 2: Enhanced Features
- [ ] Real-time notifications
- [ ] File upload for leads import
- [ ] Email template builder
- [ ] Campaign analytics
- [ ] Third-party integrations (HubSpot, Salesforce, etc.)

### Phase 3: Production
- [ ] Minify & optimize assets
- [ ] Add error boundaries
- [ ] Implement error logging
- [ ] Add analytics tracking
- [ ] Security: HTTPS, CSRF protection, XSS prevention

## 📞 Support

For issues or questions:
1. Check browser console for errors
2. Verify all CSS files are loading
3. Check localStorage data with DevTools
4. Ensure JavaScript files are linked correctly

## 📄 License

MIT – Feel free to use for personal or commercial projects.

---

**Built with ❤️ for modern sales teams**

LeadPilot © 2025
