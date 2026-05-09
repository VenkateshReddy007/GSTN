# GSTN Regulatory Portal (Mock)

A mock portal demonstrating GST Network regulatory data management for RegGraph AI demo purposes.

## Features

- Static HTML-based regulatory portal
- JSON-based regulation database
- Responsive table display of regulations
- Mock data with version tracking and hash verification

## Project Structure

- `index.html` - Main portal interface
- `regulations.json` - Regulatory data with version control
- `package.json` - Project metadata
- `vercel.json` - Vercel deployment configuration

## Getting Started

### Prerequisites
- A modern web browser
- (Optional) Node.js for local development server

### Running Locally

Open `index.html` directly in your browser, or use a local server:

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js (http-server)
npx http-server
```

Then navigate to `http://localhost:8000` (or appropriate port).

## Deployment

### Vercel (Recommended)

The project is configured for Vercel deployment with `vercel.json`.

1. Connect repository to Vercel
2. Vercel will automatically detect the static site configuration
3. Deploy to: `https://gstn.vercel.app`

### Manual Deployment

1. Build the project (if applicable)
2. Deploy static files to your hosting service
3. Ensure CORS headers are properly configured for JSON requests

## Data Format

The `regulations.json` file contains:
- Version information
- Last updated timestamp
- Hash check for data integrity
- Array of regulation records with:
  - ID, Title, Category
  - Value and Unit
  - Effective Date
  - Applicable States
  - Description

## License

Mock project for demonstration purposes.