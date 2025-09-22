# Instagram (instagram-mern)

Full-stack Instagram-like social media app (MERN stack). Backend Node/Express + MongoDB, frontend React. Features include user auth, posting images, likes, comments, file uploads via multer/AWS S3, realtime notifications with socket.io, and email support via SendGrid.

## Tech stack
- Node.js, Express
- MongoDB (Mongoose)
- React (frontend folder)
- AWS S3 (multer-s3) for media
- Socket.io for realtime
- SendGrid for emails
- JWT for auth
- bcrypt for password hashing

## Quick setup (development)
1. Install dependencies
   - Root:
     npm install
   - Frontend:
     npm install --prefix frontend

2. Environment variables
   Create a `.env` in root with keys required by the server (MONGO_URI, JWT_SECRET, AWS keys, SENDGRID_API_KEY, etc). Do NOT commit `.env`.

3. Run server (dev)
   npm run dev

4. Run frontend (dev)
   npm start --prefix frontend

## Deployment
- Build frontend:
  npm run build --prefix frontend
- Production start:
  npm start

## Notes
- .gitignore excludes secrets and node_modules.
- Use the `heroku-postbuild` script for Heroku deployment.

## License
MIT
