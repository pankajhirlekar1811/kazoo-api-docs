# 2600Hz Kazoo API - Complete Swagger Documentation

## Files
- `kazoo-api-complete.yaml` - Complete OpenAPI 3.0 specification with all 633 endpoints
- `index.html` - Swagger UI viewer
- `README.md` - This file

## How to View

### Option 1: Local Web Server (Recommended)
1. Open a terminal in this directory
2. Run: `python -m http.server 8080` (Python 3) or `python -m SimpleHTTPServer 8080` (Python 2)
3. Open browser: http://localhost:8080

### Option 2: Online Swagger Editor
1. Go to https://editor.swagger.io/
2. File → Import File → Select `kazoo-api-complete.yaml`

### Option 3: VS Code Extension
1. Install "Swagger Viewer" extension
2. Right-click `kazoo-api-complete.yaml` → Preview Swagger

## API Overview

### Total Endpoints: 633

- **DELETE**: 76 endpoints
- **GET**: 310 endpoints  
- **PATCH**: 46 endpoints
- **POST**: 111 endpoints
- **PUT**: 90 endpoints

### Main Categories

- **Accounts** - Account management and configuration
- **Devices** - Device provisioning and management
- **Users** - User management and authentication
- **Callflows** - Call routing and flows
- **Phone Numbers** - Number management and porting
- **Voicemail** - Voicemail boxes and messages
- **Faxes** - Fax sending and receiving
- **Media** - Media files and prompts
- **CDRs** - Call detail records
- **Webhooks** - Event notifications
- **Qubicle/ACDC** - Call center queues and agents (62 endpoints)
- **Authentication** - Token and user authentication
- **Services** - Billing and services
- **System** - System configuration and status

## Authentication

All APIs require authentication using:
- **X-Auth-Token** header (API Key)
- **Bearer Token** (OAuth)

Get an auth token:
```bash
curl -X PUT https://api.2600hz.com/v2/user_auth \
  -H "Content-Type: application/json" \
  -d '{"data":{"credentials":"USERNAME:PASSWORD","account_name":"ACCOUNT_NAME"}}'
```

## Source

Generated from: https://docs.2600hz.com/

All 633 APIs scraped and documented from official 2600Hz Kazoo documentation.
