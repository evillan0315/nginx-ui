# Nginx UI

A simple user interface for managing Nginx configurations with Next.js, MUI, and TypeScript. This application allows you to:
- Perform CRUD operations for domains
- Configure domain settings
- Automate SSL creation with Let's Encrypt

## Features
- 📌 **Manage Domains**: Add, update, and delete domain configurations
- ⚙️ **Nginx Configuration**: Modify and reload Nginx settings
- 🔐 **SSL Automation**: Enable SSL certificates via Let's Encrypt

## Tech Stack
- **Frontend**: Next.js, TypeScript, MUI
- **Backend**: Express.js, Node.js
- **Tools**: Certbot (Let's Encrypt), Nginx, Docker (optional)

## Installation
### Prerequisites
Ensure you have the following installed:
- Node.js
- Nginx
- Certbot (Let's Encrypt)

### Clone the Repository
```bash
git clone https://github.com/evillan0315/nginx-ui.git
cd nginx-ui
```

### Install Dependencies
#### Backend
```bash
cd backend
npm install
```
#### Frontend
```bash
cd frontend
npm install
```

## Usage
### Start Backend
```bash
cd backend
npm run dev
```

### Start Frontend
```bash
cd frontend
npm run dev
```

## API Endpoints
### Add a Domain
```http
POST /domains
```
**Body:**
```json
{
  "domain": "example.com",
  "config": "nginx configuration string"
}
```

### Enable SSL
```http
POST /domains/:domain/ssl
```

## Future Enhancements
- UI improvements for domain listing
- Database integration for persistent storage
- Enhanced error handling and validation

## License
MIT

---
🚀 Developed by Eddie Villanueva

