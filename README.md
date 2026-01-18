# NomadLife Analytics Dashboard

An animated, real-time analytics dashboard built with React, Recharts, and Framer Motion.

## Features

- **Animated KPI Cards** - Counting animations for key metrics
- **Interactive Charts** - Area charts, bar charts, and pie charts
- **Glassmorphism Design** - Modern dark theme with blur effects
- **Real-time Data** - Connected to backend API for live statistics

## Tech Stack

- React 18
- Recharts
- Framer Motion
- Tailwind CSS
- Lucide React Icons

## Installation

```bash
npm install recharts framer-motion lucide-react
```

## Usage

```jsx
import AnalyticsDashboard from './AnalyticsDashboard';

// Fetch analytics from your API
const analytics = await fetch('/api/analytics').then(r => r.json());

// Render the dashboard
<AnalyticsDashboard analytics={analytics} />
```

## Data Structure

```typescript
interface Analytics {
  totalUsers: number;
  premiumUsers: number;
  totalPosts: number;
  totalBookings: number;
  totalMessages: number;
  totalPlaces: number;
  usersByMonth: { month: string; count: number }[];
  postsByCity: { city: string; count: number }[];
  bookingsByStatus: { status: string; count: number }[];
  recentActivity: { date: string; users: number; posts: number; bookings: number }[];
}
```

## License

MIT