# Blog Platform

A full-stack blogging platform where users can create posts, interact with other users, and build a community around shared content.
[Live Demo](https://heet-113.github.io/Blog-platform-frontend/)
## Project Overview

This is a complete MERN (MongoDB, Express, React, Node.js) stack application featuring:

- **User Authentication**: Secure registration and login with JWT
- **Blog Posts**: Create, read, update, and delete posts
- **Comments**: Interactive comments section on each post
- **RESTful API**: Backend API for all operations

## Features

✅ User registration, login, and authentication  
✅ Create, edit, delete blog posts  
✅ Comment section for user interaction  
✅ Backend with RESTful APIs and database integration  
✅ Frontend deployed on GitHub Pages  
✅ Backend deployed on Render  

## Project Structure

```
Blog-platform/
├── backend/                  # Node.js Express API
│   ├── models/              # MongoDB schemas
│   ├── routes/              # API endpoints
│   ├── middleware/          # Authentication middleware
│   ├── server.js            # Server entry point
│   ├── package.json         # Dependencies
│   └── .env.example         # Environment variables
│
└── frontend/                # React Application
    ├── src/
    │   ├── components/      # Reusable components
    │   ├── pages/          # Page components
    │   ├── App.js          # Main app
    │   └── index.js        # Entry point
    ├── public/             # Static files
    └── package.json        # Dependencies
```

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- MongoDB (local or Atlas)
- npm or yarn

### Backend Setup

1. Navigate to the backend folder:
```bash
cd backend
```

2. Install dependencies:
```bash
npm install
```

3. Create `.env` file with:
```
MONGODB_URI=mongodb://localhost:27017/blog-platform
JWT_SECRET=your_jwt_secret_key_here
PORT=5000
NODE_ENV=development
```

4. Start the server:
```bash
npm run dev
```

Server runs on `http://localhost:5000`

### Frontend Setup

1. Navigate to the frontend folder:
```bash
cd frontend
```

2. Install dependencies:
```bash
npm install
```

3. Create `.env` file with:
```
REACT_APP_API_URL=http://localhost:5000/api
```

4. Start the development server:
```bash
npm start
```

Application opens at `http://localhost:3000`

## API Endpoints

### Authentication
- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - Login user

### Posts
- `GET /api/posts` - Get all posts
- `GET /api/posts/:id` - Get single post
- `POST /api/posts` - Create post (authenticated)
- `PUT /api/posts/:id` - Update post (authenticated)
- `DELETE /api/posts/:id` - Delete post (authenticated)

### Comments
- `GET /api/comments/:postId` - Get comments for a post
- `POST /api/comments/:postId` - Create comment (authenticated)
- `DELETE /api/comments/:commentId` - Delete comment (authenticated)

## Deployment

### Backend (Render)
1. Push code to GitHub
2. Connect repository to Render
3. Set environment variables in Render dashboard
4. Deploy

### Frontend (GitHub Pages)
1. Update `homepage` in `package.json` with your GitHub Pages URL
2. Install gh-pages: `npm install --save-dev gh-pages`
3. Deploy: `npm run deploy`

## Technologies Used

**Backend:**
- Node.js
- Express.js
- MongoDB
- Mongoose
- JWT Authentication
- bcryptjs (password hashing)

**Frontend:**
- React
- React Router
- Axios
- CSS3

## Learning Outcomes

By building this project, you'll learn:
- Full-stack development with MERN
- RESTful API design and implementation
- User authentication and authorization
- Database modeling with MongoDB
- State management in React
- Deployment strategies
- Frontend and backend integration

## Future Enhancements

- User profiles
- Post likes/reactions
- Search functionality
- Categories/Tags
- Email notifications
- Social sharing features
- Rich text editor for posts

## Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest features
- Submit pull requests

## License

This project is open source and available under the MIT License.

## Support

For issues or questions:
1. Check existing issues in the repository
2. Create a new issue with detailed description
3. Include error messages and code snippets

Happy blogging! 📝
