# MyPortal - Developer Advocate Portfolio Site

A modern, responsive portfolio website built for showcasing development and technical advocacy skills. This project uses a clean HTML/CSS design with Docker containerization for easy deployment.

## ? Overview

This portfolio website is designed for Arsheen Kour, a Software Testing Engineer, featuring:

- Responsive design that works on mobile, tablet, and desktop devices
- Modern blue theme with professional styling
- Sections for About, Experience, Projects, Skills, Education, and Contact
- Docker containerization for consistent deployment

## ?? Technologies Used

- **Frontend**: HTML5, CSS3, JavaScript
- **Icons**: Font Awesome
- **Fonts**: Google Fonts (Poppins)
- **Containerization**: Docker and Docker Compose
- **Web Server**: Nginx

## ? Getting Started

### Prerequisites

- Docker and Docker Compose installed on your system

### Running Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/ajeetraina/myportal.git
   cd myportal
   ```

2. Build and run the Docker container:
   ```bash
   docker-compose up -d
   ```

3. Visit `http://localhost:8080` in your browser

### Development Mode

The Docker Compose configuration includes volume mounting for development:
- Source files are mounted to the container for hot-reloading
- Nginx configuration is mounted to ensure proper server setup

## ? Project Structure

- `index.html` - Main portfolio page
- `css/` - Stylesheet directory
- `js/` - JavaScript functionality
- `nginx.conf` - Web server configuration
- `Dockerfile` - Container build instructions
- `docker-compose.yml` - Container orchestration
- `.dockerignore` - Files excluded from container build

## ? Docker Configuration

The project is containerized using:

- Alpine-based Nginx image for a small footprint
- Custom Nginx configuration for performance and security
- Docker Compose for easy local development and deployment
- Health checks to ensure service availability

## ? Deployment

The site can be deployed:

1. As a Docker container on any Docker-compatible hosting
2. On GitHub Pages using the static HTML/CSS files
3. On any web server by copying the static files

## ? Security

The Nginx configuration includes:
- GZIP compression for better performance
- Content Security Policy (CSP) headers
- X-Content-Type-Options and X-XSS-Protection headers
- Custom error pages (404, 500, etc.)

## ? License

This project is available for personal use and modification. Please contact the original author for commercial usage.

## ? Author

Arsheen Kour - Software Testing Engineer

## ? Acknowledgments

- Font Awesome for icons
- Google Fonts for typography
- Docker and Nginx for infrastructure
