# ChainFactor - Web3 Invoice Factoring Dashboard

A modern, responsive Web3 dashboard UI for blockchain invoice factoring built with Next.js, React, and TailwindCSS.

## Features

### 🎨 Design System
- **Dark Theme**: Professional dark mode with glassmorphism effects
- **Responsive Design**: Fully mobile-friendly with Tailwind CSS breakpoints
- **Modern Components**: Reusable React components with smooth animations
- **Professional Styling**: Enterprise-grade fintech UI inspired by leading DeFi platforms

### 📄 Pages

1. **Landing Page** (`/`)
   - Hero section explaining blockchain invoice factoring
   - Feature showcase (Mirror Invoice System, AI Risk Scoring, Smart Contract Settlement)
   - How It Works section (4-step process)
   - Call-to-action section
   - Footer with navigation

2. **Invoice Marketplace** (`/marketplace`)
   - Responsive grid of invoice cards
   - Filter invoices by risk level (Low, Medium, High)
   - Real-time auction countdown timer
   - Investment action buttons
   - Statistics dashboard

3. **Investor Portfolio** (`/portfolio`)
   - Key statistics cards (Total Invested, Active Invoices, Total Yield, Avg Risk)
   - Earnings chart over time
   - Risk distribution pie chart
   - Active investments table
   - Upcoming repayments section

4. **Business Dashboard** (`/business`)
   - Upload Mirror Invoice form
   - Business statistics overview
   - Cash flow projection chart
   - Invoice status distribution pie chart
   - Active invoices management table
   - Funding status indicators

5. **Invoice Detail Page** (`/invoice/[id]`)
   - Comprehensive invoice information
   - Risk score visualization
   - Payment history timeline
   - Auction countdown timer
   - Investor distribution table
   - Funding status and progress bar

### 🧩 Reusable Components

#### Layout Components
- `Navbar`: Fixed navigation with wallet connection
- `Sidebar`: Collapsible side navigation
- `MainLayout`: Main layout wrapper with navbar and sidebar

#### Common Components
- `WalletConnectButton`: Web3 wallet connection (mock)
- `RiskScoreBadge`: Risk level indicator (Low/Medium/High)
- `AuctionTimer`: Countdown timer for auction deadlines

#### Card Components
- `StatisticCard`: KPI statistics display
- `InvoiceCard`: Invoice details with investment button

#### Chart Components
- `LineChart`: Time series data visualization
- `BarChart`: Comparative data visualization
- `DoughnutChart`: Distribution data with center value

## Tech Stack

- **Framework**: Next.js 16.x with App Router
- **Language**: TypeScript
- **Styling**: TailwindCSS v4
- **UI**: React 19.x
- **Dev Tools**: ESLint

## Getting Started

### Prerequisites
- Node.js 18.x or higher
- npm, yarn, pnpm, or bun

### Installation

```bash
# Install dependencies
npm install

# Run development server
npm run dev

# Open in browser
# Visit http://localhost:3000
```

### Build for Production

```bash
# Build the application
npm run build

# Start production server
npm start
```

### Linting

```bash
# Run ESLint
npm run lint
```

## Project Structure

```
src/
├── app/
│   ├── layout.tsx              # Root layout
│   ├── globals.css             # Global styles
│   ├── page.tsx                # Landing page
│   ├── marketplace/
│   │   └── page.tsx            # Marketplace page
│   ├── portfolio/
│   │   └── page.tsx            # Portfolio dashboard
│   ├── business/
│   │   └── page.tsx            # Business dashboard
│   └── invoice/
│       └── [id]/
│           └── page.tsx        # Invoice detail page
├── components/
│   ├── layout/
│   │   ├── MainLayout.tsx      # Main layout wrapper
│   │   └── Sidebar.tsx         # Sidebar navigation
│   ├── common/
│   │   ├── Navbar.tsx          # Top navigation
│   │   ├── WalletConnectButton.tsx
│   │   ├── RiskScoreBadge.tsx
│   │   └── AuctionTimer.tsx
│   ├── cards/
│   │   ├── StatisticCard.tsx
│   │   └── InvoiceCard.tsx
│   └── charts/
│       ├── LineChart.tsx
│       ├── BarChart.tsx
│       └── DoughnutChart.tsx
```

## Styling Features

### Glassmorphism
- `.glass` - Glassmorphism background with backdrop blur
- `.glass-dark` - Dark glassmorphism variant

### Gradients & Effects
- `.gradient-text` - Gradient text effect
- `.shadow-glow` - Indigo glow shadow
- `.shadow-lg-glow` - Large indigo glow shadow
- `.hover-lift` - Hover scale and glow effect

### Risk Scoring Colors
- `.risk-low` - Green badge for low risk
- `.risk-medium` - Yellow badge for medium risk
- `.risk-high` - Red badge for high risk

### Utilities
- `.transition-smooth` - Smooth transitions (300ms)
- `.gradient-bg` - Dark gradient background

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Performance

- **SSR & SSG**: Next.js App Router with SSR support
- **Image Optimization**: Next.js Image component ready
- **Code Splitting**: Automatic by Next.js
- **CSS**: TailwindCSS with production purging

## Customization

### Colors
Edit CSS variables in `src/app/globals.css`:

```css
:root {
  --primary: #6366f1;
  --success: #10b981;
  --warning: #f59e0b;
  --danger: #ef4444;
}
```

### Theme
The app uses a dark theme by default. To customize:

1. Modify color scheme in `globals.css`
2. Update Tailwind classes in components
3. Adjust glow and shadow effects

## Future Enhancements

- Web3 wallet integration (MetaMask, WalletConnect)
- Real blockchain data integration
- WebSocket real-time updates
- More interactive charts (D3.js, Recharts)
- Payment gateway integration
- Mobile app native version
- Advanced analytics dashboard

## License

MIT License - feel free to use this template for your projects

## Support

For questions or issues, please review the code and component structure or consult Next.js and TailwindCSS documentation.

---

**ChainFactor** - Turn unpaid invoices into instant liquidity using blockchain. ⚡
