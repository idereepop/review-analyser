# Customer Reviews Dashboard

A powerful, AI-driven web application that analyzes customer reviews and provides actionable business insights through an interactive dashboard. Built with Next.js, React, and integrated with Scoutos AI API for advanced natural language processing.

## 🎯 Features

### Sentiment Analysis
- Automatically classify customer reviews as positive, neutral, or negative
- Track sentiment trends over time with interactive visualizations
- Identify emotional patterns in customer feedback

### Aspect Analysis
- Extract and categorize specific aspects of your product/service mentioned in reviews
- Analyze sentiment for each aspect independently (customer service, pricing, delivery, product quality, usability)
- Discover which features resonate most with customers

### Recurring Issues Detection
- Automatically identify the most frequently mentioned problems
- Prioritize issues by impact and frequency
- Get actionable recommendations for addressing top concerns

### Feature Requests
- Extract and track customer feature requests from reviews
- Prioritize requests based on frequency and customer demand
- Make data-driven product roadmap decisions

### Competitor Insights
- Identify positive traits customers associate with competitors
- Discover market opportunities and competitive advantages
- Understand what customers value in competing solutions

### Actionable Recommendations
- Receive AI-generated recommendations based on comprehensive review analysis
- Get specific, prioritized action items for business improvement
- Make informed decisions backed by customer feedback

## 🚀 Technologies

### Frontend
- **Next.js 14** - React framework with API routes and server-side rendering
- **React 19** - UI library with hooks and server components
- **Tailwind CSS** - Utility-first CSS framework for responsive design
- **Framer Motion** - Animation library for smooth interactions
- **Shadcn/UI** - Accessible, customizable React components

### Data Visualization
- **Chart.js** - Lightweight charting library
- **React-chartjs-2** - React wrapper for Chart.js
- **React Circular Progressbar** - Circular progress indicators

### AI Integration
- **Scoutos AI API** - Advanced LLM-powered text analysis
- Server-side API integration for secure key management

### Styling & Theme
- **Tailwind CSS** with dark mode support
- Custom CSS utilities for glass-morphism effects
- Responsive design for all device sizes

## 🛠️ Getting Started

### Prerequisites
- Node.js 16+ and npm/yarn
- Scoutos API key (get one from [scoutos.com](https://scoutos.com))

### Installation

1. Clone the repository
\`\`\`bash
git clone <repository-url>
cd customer-reviews-dashboard
\`\`\`

2. Install dependencies
\`\`\`bash
npm install
\`\`\`

3. Set up environment variables
Create a `.env.local` file in the project root:
\`\`\`
SCOUTOS_API_KEY=your_api_key_here
NEXT_PUBLIC_DEV_SUPABASE_REDIRECT_URL=http://localhost:3000
\`\`\`

4. Run the development server
\`\`\`bash
npm run dev
\`\`\`

5. Open [http://localhost:3000](http://localhost:3000) in your browser

## 📁 Project Structure

\`\`\`
├── app/
│   ├── components/
│   │   ├── Dashboard.tsx          # Main dashboard with all visualizations
│   │   ├── FileUpload.tsx         # File upload component
│   ├── api/
│   │   └── upload/
│   │       └── route.ts           # API endpoint for Scoutos AI processing
│   ├── dashboard/
│   │   ├── page.tsx               # Dashboard page
│   │   └── loading.tsx            # Loading state
│   ├── page.tsx                   # Home page with file upload
│   ├── layout.tsx                 # Root layout
│   └── globals.css                # Global styles
├── components/
│   ├── ui/                        # Shadcn/UI components
│   └── theme-provider.tsx         # Dark mode provider
├── documentation/                 # Project documentation
│   ├── diploma-thesis.md          # Complete thesis document
│   ├── bar-charts.md              # Bar charts documentation
│   ├── chart-examples.md          # Chart implementation examples
│   ├── code-descriptions.md       # Code functionality descriptions
│   └── actual-chart-implementations.md # Real implementations from dashboard
└── public/                        # Static assets
\`\`\`

## 🎨 Dashboard Components

### Sentiment Tab
- Pie chart showing sentiment distribution
- Interactive sentiment breakdown with example comments
- Overall sentiment indicator (Mostly Positive/Negative/Mixed)

### Aspects Tab
- Stacked bar chart comparing positive/negative sentiment by aspect
- Interactive cards for each aspect showing detailed metrics
- Expandable section with customer comments per aspect

### Issues Tab
- Circular progress indicators for recurring issues
- Top issues ranked by impact
- Feature requests with priority levels and trend analysis

### Recommendations Tab
- Numbered action cards with specific recommendations
- Context from customer feedback
- Prioritized based on frequency and impact

## 📊 Data Flow

1. User uploads a text file containing customer reviews
2. File is sent to `/api/upload` endpoint
3. API sends data to Scoutos AI for processing
4. Structured analysis results are returned
5. Dashboard visualizes the data through interactive charts and cards
6. User can explore insights, filter, and export findings

## 🔒 Security

- API keys are stored as environment variables and never exposed to the client
- API route acts as a secure proxy between frontend and Scoutos AI
- All data processing happens server-side
- Input validation on both client and server

## 📈 Performance

- Responsive design optimized for mobile, tablet, and desktop
- Smooth animations with Framer Motion
- Efficient data visualization with Chart.js
- Progressive UI updates with loading states
- Optimized images and asset delivery

## 🌙 Theme Support

The application includes built-in dark mode support with:
- System theme detection
- Manual theme toggle
- Persistent theme preference
- Optimized colors for readability in both modes

## 📝 Documentation

Complete project documentation is available in the `documentation/` folder:
- Detailed thesis document with architecture and implementation details
- Chart visualization examples and explanations
- Code descriptions for each component
- Actual implementations from the dashboard

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is part of a diploma thesis and is provided as-is for educational purposes.

## 🎓 Academic Project

This application was developed as part of a diploma project focusing on:
- Advanced web application development with Next.js and React
- Integration with AI APIs for text analysis
- Data visualization and user interface design
- Full-stack application architecture
- Real-world business problem solving

For detailed technical information, see the thesis documentation in the `documentation/` folder.

---

**Built with ❤️ using Next.js, React, and Scoutos AI**
