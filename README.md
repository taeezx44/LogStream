# LogStream - Distributed Log Search Engine

A modern, real-time log monitoring and analytics dashboard built with vanilla HTML, CSS, and JavaScript.

## Features

- **Real-time Log Streaming**: Live log ingestion and display
- **Advanced Search**: Full-text search with filters for level, service, host, and time ranges
- **Interactive Analytics**: Charts and visualizations for log metrics
- **Agent Simulation**: Simulate multiple log agents generating data
- **Bulk Import**: Import logs via JSON arrays
- **API Documentation**: Built-in API reference
- **Responsive Design**: Works on desktop and mobile devices

## Quick Start

### Deploy to Vercel

1. Install Vercel CLI:
```bash
npm i -g vercel
```

2. Deploy:
```bash
vercel
```

Or connect your GitHub repository to Vercel for automatic deployments.

### Local Development

1. Clone this repository
2. Run a local server:
```bash
# Using Python
python -m http.server 3000

# Using Node.js
npx serve .

# Or use the package.json script
npm start
```

3. Open `http://localhost:3000` in your browser

## Project Structure

```
├── index.html          # Main application
├── vercel.json         # Vercel configuration
├── package.json         # Project metadata
└── README.md          # This file
```

## Configuration

### Vercel Configuration

The `vercel.json` file handles:
- Single Page Application routing
- Static asset caching
- HTML cache control

### Environment Variables

This is a static application and doesn't require environment variables.

## API Endpoints

The application includes a mock API interface with the following endpoints:

- `POST /api/v1/logs/ingest` - Ingest single log entry
- `POST /api/v1/logs/bulk` - Bulk ingest logs
- `GET /api/v1/logs/search` - Search logs with filters
- `GET /api/v1/logs/stream` - Real-time SSE stream
- `GET /api/v1/logs/stats` - Aggregated statistics
- `DELETE /api/v1/logs` - Delete logs by query

## Deployment

### Vercel Deployment

1. Push your code to GitHub
2. Connect your repository to [Vercel](https://vercel.com)
3. Vercel will automatically detect and deploy your static site
4. Your site will be available at `https://your-project-name.vercel.app`

### Manual Deployment

You can also deploy manually:

```bash
vercel --prod
```

## Technologies Used

- **HTML5** - Semantic markup
- **CSS3** - Modern styling with CSS Grid and Flexbox
- **Vanilla JavaScript** - No framework dependencies
- **Chart.js** - Data visualization (via CDN)
- **Google Fonts** - Typography

## Browser Support

- Chrome 80+
- Firefox 75+
- Safari 13+
- Edge 80+

## License

MIT License - see LICENSE file for details.

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## Support

For issues and questions, please open an issue on the GitHub repository.
