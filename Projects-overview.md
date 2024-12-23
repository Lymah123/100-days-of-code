# Project 1: PERSONAL DOCUMENT VAULT

## A personal document vault with an encryption project

## Project Overview
Objective: Build a secure document vault where users can upload, organize, search, and delete documents. All documents must be encrypted before being stored in AWS S3, and users must authenticate to access their files. Use React for the frontend, Node.js with MongoDB for the backend, Crypto.js for encryption, and AWS S3 for storage.

Feature Breakdown
1. User Authentication and Access Control
Purpose: Ensure only authorized users can access the system.
Implementation:
Backend: Use bcrypt for password hashing and JSON web token for user sessions.
Frontend: React for login/signup forms and session handling (via cookies/local storage).
2. Upload Documents
Purpose: Allow users to upload files to AWS S3 securely.
Steps:
Use Crypto.js to encrypt the file on the server before uploading it to S3.
Ensure S3 stores only the encrypted version of the document.
Dependencies: multer (for file uploads), crypto, @aws-sdk/client-s3.
3. Organize Documents
Purpose: Allow users to group or tag documents for better organization.
Steps:
Store metadata (e.g., tags, names, user reference) in MongoDB.
Associate uploaded files with the authenticated user in the database.
4. Search Functionality
Purpose: Allow users to search their uploaded documents.
Steps:
Use MongoDB's text indexing for searching document metadata (e.g., tags, names).
Provide a search bar in the frontend to query the backend.
5. End-to-End Encryption
Purpose: Encrypt all documents for privacy and security.
Steps:
Use crypto.createCipheriv() and crypto.createDecipheriv() to encrypt and decrypt files.
Use a secure key (per user or global for the application) stored safely in an environment variable.

## Backend Plan

### Folder Structure

backend/
├── config/
│   ├── db.js            # MongoDB connection setup
│   ├── s3.js            # AWS S3 client and upload logic
├── controllers/
│   ├── authController.js      # Handles user authentication
│   ├── documentController.js  # Handles upload, encryption, organization, and search
├── middleware/
│   ├── authMiddleware.js  # Middleware for verifying user authentication
├── models/
│   ├── user.js            # MongoDB schema for users
│   ├── document.js        # MongoDB schema for documents
├── routes/
│   ├── auth.js            # User authentication routes
│   ├── upload.js          # Document upload routes
├── utils/
│   ├── cryptoUtils.js     # File encryption and decryption logic
├── .env                  # Environment variables (AWS, MongoDB, JWT keys)
├── server.js             # Main server entry point

## Frontend Plan
### Folder structure
frontend/
├── src/
│   ├── components/
│   │   ├── Auth/
│   │   ├── Dashboard/
│   │   ├── DocumentUpload/
│   │   ├── Search/
│   ├── pages/
│   │   ├── Login.js
│   │   ├── Register.js
│   │   ├── Dashboard.js
│   ├── utils/
│   │   ├── api.js # Axios API functions


### Frontend Key Features
Authentication:

Store JWT in local storage or cookies.
Redirect unauthorized users to login.
Upload Documents:

Create a React component with a file input and metadata fields (tags, file name).
Use Axios to send the file to /api/upload.
Search and Organize:

Create a search bar to filter documents by metadata.
Display documents in a user-friendly dashboard.
Next Steps
Set up backend authentication and routes.
Integrate document upload with encryption and S3 storage.
Build React components for authentication, upload, and dashboard.
Implement search and tagging.
