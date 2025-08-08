# Deployment Guide

## Quick Fix for Current Error

The error you're seeing is because there's no `package-lock.json` file. Here's how to fix it:

### Option 1: Generate package-lock.json locally
\`\`\`bash
# Delete node_modules if it exists
rm -rf node_modules

# Install dependencies to generate package-lock.json
npm install

# Commit the new package-lock.json
git add package-lock.json
git commit -m "Add package-lock.json"
git push
\`\`\`

### Option 2: Use the provided package-lock.json
1. Copy the `package-lock.json` file from this project
2. Add it to your repository root
3. Commit and push:
\`\`\`bash
git add package-lock.json
git commit -m "Add package-lock.json for deployment"
git push
\`\`\`

## Deployment Options

### 1. Vercel (Recommended)
1. Go to [vercel.com](https://vercel.com)
2. Connect your GitHub repository
3. Deploy automatically

### 2. Netlify
1. Go to [netlify.com](https://netlify.com)
2. Connect your GitHub repository
3. Build settings:
   - Build command: `npm run build`
   - Publish directory: `.next`

### 3. GitHub Pages (Static Export)
Add to `next.config.js`:
\`\`\`javascript
/** @type {import('next').NextConfig} */
const nextConfig = {
  output: 'export',
  trailingSlash: true,
  images: {
    unoptimized: true
  }
}

module.exports = nextConfig
\`\`\`

## Environment Variables (Optional)

For database integration, add these to your deployment platform:
\`\`\`
NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
SUPABASE_SERVICE_ROLE_KEY=your_service_role_key
\`\`\`

## Build Commands

- **Development**: `npm run dev`
- **Production Build**: `npm run build`
- **Start Production**: `npm start`
- **Type Check**: `npm run type-check`

## Troubleshooting

### Common Issues:
1. **Missing package-lock.json**: Use the provided file or run `npm install`
2. **Node version**: Ensure Node.js 18+ is being used
3. **Build errors**: Run `npm run type-check` to check for TypeScript errors

### GitHub Actions Setup:
1. The `.github/workflows/deploy.yml` file is included
2. For Vercel deployment, add these secrets to your GitHub repository:
   - `VERCEL_TOKEN`
   - `ORG_ID`
   - `PROJECT_ID`
\`\`\`

```eslintrc.json file=".eslintrc.json"
{
  "extends": "next/core-web-vitals"
}
