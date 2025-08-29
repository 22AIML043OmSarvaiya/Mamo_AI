# 🗄️ Database Setup Guide

## Overview
This project uses **JSON Server** as a simple database solution for development and demonstration purposes. It provides a full REST API with CRUD operations.

## 🚀 Quick Start

### Option 1: Run Both Servers Together (Recommended)
```bash
npm run dev
```
This will start both:
- React App on `http://localhost:3000` (or next available port)
- JSON Database Server on `http://localhost:3001`

### Option 2: Run Servers Separately
```bash
# Terminal 1 - Database Server
npm run db

# Terminal 2 - React App
npm start
```

## 📊 Database Structure

The database (`db.json`) contains the following collections:

### Users
- `id`: Unique identifier
- `name`, `email`, `password`: Basic auth info
- `age`, `gender`, `weight`, `height`: Profile data
- `language`: Preferred language
- `createdAt`, `updatedAt`: Timestamps

### Health Data
- Daily metrics: `dailySteps`, `sleepHours`, `waterIntake`
- Health indicators: `dietQuality`, `exerciseMinutes`, `heartRate`
- Associated with `userId`

### AI Responses
- Stores all AI interactions by category
- `category`: symptoms, nutrition, fitness, etc.
- `query` and `response`: The conversation data

### Medications
- Medicine reminders and tracking
- `name`, `dosage`, `frequency`, `time`
- Active/inactive status

### Emergency Contacts
- Emergency numbers and healthcare providers
- Categorized by type (emergency, doctor, hospital)

## 🔧 API Endpoints

Base URL: `http://localhost:3001`

### Users
- `GET /users` - Get all users
- `POST /users` - Create user
- `GET /users/:id` - Get user by ID
- `PATCH /users/:id` - Update user

### Health Data
- `GET /healthData?userId=:id` - Get user's health data
- `POST /healthData` - Save health data
- `GET /healthData?userId=:id&_sort=date&_order=desc` - Latest data

### AI Responses
- `GET /aiResponses?userId=:id&category=:category` - Get responses
- `POST /aiResponses` - Save AI response

## 🎯 Features

### ✅ What's Working
- **User Authentication**: Login/Signup with database validation
- **Data Persistence**: All user data saved to database
- **AI Response Storage**: Chat history preserved
- **Real-time Status**: Database connection indicator
- **Data Export**: Download all user data

### 🚀 Database Service Features
- **CRUD Operations**: Full Create, Read, Update, Delete
- **Relationships**: User data linked by userId
- **Search & Filter**: Query by date, category, status
- **Bulk Operations**: Save multiple records
- **Health Checks**: Monitor database connectivity

## 🛠️ Customization

### Add New Collections
1. Add to `db.json`:
```json
{
  "newCollection": [
    {
      "id": "1",
      "userId": "1",
      "data": "example"
    }
  ]
}
```

2. Add methods to `databaseService.js`:
```javascript
async saveNewData(userId, data) {
  // Implementation
}
```

### Production Database
For production, replace JSON Server with:
- **PostgreSQL** with Prisma ORM
- **MongoDB** with Mongoose
- **Firebase Firestore**
- **Supabase** (PostgreSQL + Auth)

## 🔍 Troubleshooting

### Database Not Connecting
1. Check if JSON Server is running on port 3001
2. Verify `db.json` file exists
3. Check console for connection errors

### Data Not Saving
1. Verify user is logged in (`state.user.id` exists)
2. Check browser network tab for failed requests
3. Ensure database service methods are called correctly

### Port Conflicts
If port 3001 is in use:
```bash
npm run db -- --port 3002
```
Then update `BASE_URL` in `databaseService.js`

## 📈 Performance Considerations

### For Development
- JSON Server is perfect for prototyping
- No setup required, works out of the box
- Great for demos and university projects

### For Production
- Consider real database solutions
- Add proper authentication and security
- Implement data validation and sanitization
- Add rate limiting and CORS policies

## 🎓 Educational Value

Perfect for AIML 4th year projects because it demonstrates:
- **Full-stack development** with React + Database
- **RESTful API design** and consumption
- **Data modeling** and relationships
- **Real-time features** and status monitoring
- **Professional development practices**

## 📝 Next Steps

1. **Run the application**: `npm run dev`
2. **Test authentication**: Sign up with demo credentials
3. **Explore features**: Use AI chatbot, symptom checker
4. **Check database**: View stored data in `db.json`
5. **Monitor status**: Watch database indicator in dashboard

---

This database setup provides a solid foundation for your health AI application while being simple enough for university evaluation! 🎉
