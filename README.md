# SpendWise
A simple Node.js, Express, and MongoDB backend project for students to learn JWT authentication and basic CRUD operations.

## Setup Instructions

### Prerequisites
- Node.js (v14+)
- MongoDB (local or Atlas)

### Installation
1. Clone the repository
2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file with:
   ```
   PORT=5000
   MONGO_URI=mongodb://localhost:27017/spendwise
   JWT_SECRET=your_secret_key_here
   ```

### Running the Server

**Option 1: Local MongoDB**
- Install and start MongoDB locally
- Run: `npm start`

**Option 2: MongoDB Atlas (Cloud)**
- Replace `MONGO_URI` in `.env` with your Atlas connection string
- Ensure your IP is whitelisted in Atlas
- Run: `npm start`

### Development
Run with auto-reload:
```bash
npm run dev
```

### API Endpoints
- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - Login user
- `GET /api/transactions` - Get all transactions
- `POST /api/transactions` - Create transaction
