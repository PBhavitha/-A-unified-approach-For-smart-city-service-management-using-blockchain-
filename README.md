# Smart City Portal with Blockchain Integration
A smart city management system that integrates blockchain technology with urban services like air quality monitoring, healthcare management, and urban activity impact analysis.

# Project Overview
This project consists of:
- Backend: Node.js + Express server
- Frontend: React.js application with Material-UI
- Blockchain Integration: Web3.js and MetaMask
- Database: MongoDB

# Prerequisites
- Node.js (v14.0.0 or higher)
- npm (v6.0.0 or higher)
- MongoDB (v4.0.0 or higher)
- MetaMask browser extension

# Installation Steps
Backend Setup
 touch .env

Add the following environment variables to .env:
. MONGODB_URI=your_mongodb_connection_string
. JWT_SECRET=your_jwt_secret
. PORT=5000

Frontend Setup:
cd client/frontend

# Install frontend dependencies
npm install

# Create frontend environment file
touch .env

Add the following to frontend .env:

REACT_APP_BACKEND_URL=http://localhost:5000
REACT_APP_WAQI_TOKEN=your_waqi_api_token
REACT_APP_OPENWEATHER_API_KEY=your_openweather_api_key

# Installation Guide:

1. System Requirements

# Node.js Installation
1. Download Node.js (v14.0.0 or higher) from (https://nodejs.org/)
2. Run the installer
3. Verify installation:
node --version
npm --version

# React Setup
1. Create React App (if starting new):
npx create-react-app@5.0.1 frontend

2. For existing project:
cd client/frontend
npm install react@18.2.0 react-dom@18.2.0 react-router-dom@6.9.0

3. Verify React installation:
npm list react
npm list react-dom

4. Start React development server:
npm start

# MongoDB Installation
1. Download MongoDB Community Server from [MongoDB website](https://www.mongodb.com/try/download/community)
2. Follow installation wizard
3. Add MongoDB to system PATH
4. Create a data directory:

mkdir C:\data\db
5. Start MongoDB service:

mongod
6. Verify MongoDB is running on mongodb://localhost:27017

# MetaMask Setup
1. Install MetaMask browser extension from (https://chrome.google.com/webstore/detail/metamask/nkbihfbeogaeaoehlefnkodbefgpgknn) 
2. Create a new wallet or import existing one
3. Connect to local blockchain network (if testing locally) or desired test network

# Backend Dependencies Installation:

Core Backend Dependencies:

1. express (^4.18.2)
   - Web application framework
   - Handles HTTP requests, routing, and middleware
   - Core of the backend server
   
   . npm install express@4.18.2

2. mongoose (^7.0.3)
   - MongoDB object modeling tool
   - Manages database connections
   - Provides schema validation
   - Handles data relationships

   . npm install mongoose@7.0.3

3. bcryptjs (^2.4.3)
   - Password hashing library
   - Secures user passwords
   - Provides salt generation and comparison functions

npm install bcryptjs@2.4.3

4. jsonwebtoken (^9.0.0)
   - Implements JWT authentication
   - Generates and verifies tokens
   - Secures API endpoints
npm install jsonwebtoken@9.0.0

5. cors (^2.8.5)
   - Enables Cross-Origin Resource Sharing
   - Required for frontend-backend communication
   - Configures allowed origins and methods
npm install cors@2.8.5

6. dotenv (^16.0.3)
   - Loads environment variables
   - Keeps sensitive data secure
   - Manages different configurations

npm install dotenv@16.0.3

Install all backend dependencies at once:
npm install express@4.18.2 mongoose@7.0.3 bcryptjs@2.4.3 jsonwebtoken@9.0.0 cors@2.8.5 dotenv@16.0.3

Development dependencies:
npm install --save-dev nodemon@2.0.22 concurrently@8.0.1

# Frontend Dependencies Installation:

   cd client/frontend

 Core Frontend Dependencies:

1. React Core:
   - react (^18.2.0) - Core React library, builds user interfaces
   - react-dom (^18.2.0) - DOM-specific React methods
   - react-router-dom (^6.9.0) - Handles routing in React applications

npm install react@18.2.0 react-dom@18.2.0 react-router-dom@6.9.0

2. Material-UI Components:
   - @mui/material (^5.16.14) - Core Material-UI components
   - @mui/icons-material (^5.16.14) - Material Design icons
   - @emotion/react (^11.14.0) - Required for MUI styling
   - @emotion/styled (^11.14.0) - Styled components for MUI

npm install @mui/material@5.16.14 @mui/icons-material@5.16.14 @emotion/react@11.14.0 @emotion/styled@11.14.0

3. Charts and Data Visualization:
   - @mui/x-charts (^7.27.1) - Material-UI charting library
   - chart.js (^4.4.8)** - Advanced charting capabilities
   - @nivo/ components - Rich data visualization

npm install @mui/x-charts@7.27.1 chart.js@4.4.8
npm install @nivo/core@0.80.0 @nivo/bar@0.80.0 @nivo/line@0.80.0 @nivo/pie@0.80.0

4. Maps Integration:
   - @react-google-maps/api (^2.18.1) - Google Maps React components
   - @tomtom-international/web-sdk-maps (^6.25.0) - TomTom maps integration
   - @tomtom-international/web-sdk-services (^6.25.0) - TomTom location services

npm install @react-google-maps/api@2.18.1 @tomtom-international/web-sdk-maps@6.25.0 @tomtom-international/web-sdk-services@6.25.0

5. Blockchain Integration:
   - @web3-react/core (^8.2.3) - React hooks for Web3
   - @web3-react/injected-connector (^6.0.7) - MetaMask connector
   - @truffle/contract (^4.6.19) - Smart contract integration

npm install @web3-react/core@8.2.3 @web3-react/injected-connector@6.0.7 @truffle/contract@4.6.19

6. Date and Time Handling:
   - date-fns (^2.30.0) - Date manipulation library
   - date-fns-tz (^2.0.0) - Timezone support

npm install date-fns@2.30.0 date-fns-tz@2.0.0

7. HTTP and API:
   - axios (^1.8.1) - HTTP client for API requests

npm install axios@1.8.1

8. Maps and Data Services:
   - axios (^1.8.1) - HTTP client for API requests

npm install axios@1.8.1

# Install all frontend dependencies at once:

npm install react@18.2.0 react-dom@18.2.0 react-router-dom@6.9.0 @mui/material@5.16.14 @mui/icons-material@5.16.14 @emotion/react@11.14.0 @emotion/styled@11.14.0 @mui/x-charts@7.27.1 chart.js@4.4.8 @nivo/core@0.80.0 @nivo/bar@0.80.0 @nivo/line@0.80.0 @nivo/pie@0.80.0 @react-google-maps/api@2.18.1 @tomtom-international/web-sdk-maps@6.25.0 @tomtom-international/web-sdk-services@6.25.0 @web3-react/core@8.2.3 @web3-react/injected-connector@6.0.7 @truffle/contract@4.6.19 date-fns@2.30.0 date-fns-tz@2.0.0 axios@1.8.1

# Environment Setup and API Keys

Backend Environment Variables (.env in root directory):

MONGODB_URI=mongodb://localhost:27017/smart_city
JWT_SECRET=your_secure_jwt_secret
PORT=5000
NODE_ENV=development

Frontend Environment Variables (.env in client/frontend):

REACT_APP_BACKEND_URL=http://localhost:5000
REACT_APP_WAQI_TOKEN=your_waqi_api_key
REACT_APP_OPENWEATHER_API_KEY=your_openweather_api_key

# Required API Keys

1. World Air Quality Index (WAQI) API Key:
   - Register at [WAQI API website](https://aqicn.org/api/)
   - Create an account
   - Generate API token
   - Add to frontend .env as REACT_APP_WAQI_TOKEN

2. OpenWeather API Key:
   - Sign up at [OpenWeather](https://openweathermap.org/api)
   - Register for a free account
   - Generate API key
   - Add to frontend .env as REACT_APP_OPENWEATHER_API_KEY

These API keys are used for:
- WAQI API: Fetching real-time air quality data
- OpenWeather API: Getting weather information and forecasts

# Development Tools

Required IDE/Editor:
- Visual Studio Code (recommended)
- Required extensions:
  - ESLint
  - Prettier
  - GitLens
  - React Developer Tools
  - MongoDB for VS Code
