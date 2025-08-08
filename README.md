# Ratnayake Project Pvt Ltd - Construction Company Website

A modern, responsive web application for Ratnayake Project Pvt Ltd, a leading construction company in Sri Lanka specializing in wall plaster, slab work, paint work, and putty work.

## Features

- **Company Showcase**: Professional homepage with company information and services
- **Subcontractor Applications**: Complete application form for contractors
- **WhatsApp Integration**: Direct messaging to company WhatsApp for applications
- **Admin Dashboard**: Manage and view applications with filtering and search
- **Mobile Responsive**: Works perfectly on all devices
- **Modern Design**: Clean, professional interface using Tailwind CSS

## Tech Stack

- **Framework**: Next.js 14 with App Router
- **Styling**: Tailwind CSS
- **UI Components**: Radix UI primitives
- **Icons**: Lucide React
- **TypeScript**: Full type safety

## Getting Started

### Prerequisites

- Node.js 18+ 
- npm or yarn

### Installation

1. Clone the repository:
\`\`\`bash
git clone https://github.com/yourusername/ratnayake-construction.git
cd ratnayake-construction
\`\`\`

2. Install dependencies:
\`\`\`bash
npm install
# or
yarn install
\`\`\`

3. Run the development server:
\`\`\`bash
npm run dev
# or
yarn dev
\`\`\`

4. Open [http://localhost:3000](http://localhost:3000) in your browser.

## Project Structure

\`\`\`
ratnayake-construction/
├── app/
│   ├── actions/          # Server actions
│   ├── admin/           # Admin dashboard
│   ├── apply/           # Application form
│   ├── globals.css      # Global styles
│   ├── layout.tsx       # Root layout
│   └── page.tsx         # Homepage
├── components/
│   └── ui/              # Reusable UI components
├── lib/
│   └── utils.ts         # Utility functions
├── public/              # Static assets
└── ...config files
\`\`\`

## Key Features

### Homepage
- Company introduction and services
- Professional about section
- Contact information
- Call-to-action for applications

### Application Form
- Comprehensive contractor application
- Service selection (Wall Plaster, Slab Work, Paint Work, Putty Work)
- WhatsApp integration for instant communication
- Form validation and user feedback

### Admin Dashboard
- View all applications
- Filter by service type
- Search functionality
- Direct WhatsApp contact with applicants
- Password protected (default: ratnayake2024)

## Contact Information

- **Company**: Ratnayake Project Pvt Ltd
- **Location**: Pannipitiya, Sri Lanka
- **Phone**: 071 444 5588
- **Email**: ratnayake72@gmail.com, ratnayakeproject@gmail.com
- **WhatsApp**: +94 77 831 3530

## Deployment

### Vercel (Recommended)

1. Push your code to GitHub
2. Connect your repository to Vercel
3. Deploy with one click

### Other Platforms

The application can be deployed to any platform that supports Next.js:
- Netlify
- Railway
- DigitalOcean App Platform
- AWS Amplify

## Environment Variables

For database integration (optional):
\`\`\`
NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
SUPABASE_SERVICE_ROLE_KEY=your_service_role_key
\`\`\`

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

This project is private and proprietary to Ratnayake Project Pvt Ltd.

## Support

For technical support or questions, please contact the development team.
