# Venge - Social Media Shopping Reviews Platform

Venge is a review platform that helps social media shoppers avoid scams by providing a place to post and read honest reviews about social media sellers.

## Features

- User authentication (signup, login, profile management)
- Post reviews with text, photos, and star ratings
- Browse and search reviews by platform, seller, or category
- Filter reviews based on different criteria
- Responsive design for both desktop and mobile

## Tech Stack

- **Frontend**: React with TypeScript and Vite
- **Styling**: Tailwind CSS
- **Backend**: Firebase (Authentication, Firestore, Storage)
- **Routing**: React Router v6

## Setup Instructions

### Prerequisites

- Node.js (v14 or newer)
- npm or yarn
- Git

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/venge.git
   cd venge
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a Firebase project:
   - Go to [Firebase Console](https://console.firebase.google.com/)
   - Create a new project
   - Add a web app to your project
   - Enable Authentication (Email/Password)
   - Create a Firestore database
   - Enable Storage

4. Set up environment variables:
   Create a `.env` file in the root directory with your Firebase configuration:
   ```
   VITE_FIREBASE_API_KEY=your-api-key
   VITE_FIREBASE_AUTH_DOMAIN=your-auth-domain
   VITE_FIREBASE_PROJECT_ID=your-project-id
   VITE_FIREBASE_STORAGE_BUCKET=your-storage-bucket
   VITE_FIREBASE_MESSAGING_SENDER_ID=your-messaging-sender-id
   VITE_FIREBASE_APP_ID=your-app-id
   ```

5. Start the development server:
   ```bash
   npm run dev
   ```

6. Open [http://localhost:5173](http://localhost:5173) in your browser

### Folder Structure

```
venge/
├── public/
├── src/
│   ├── components/
│   │   ├── auth/
│   │   │   ├── Login.tsx
│   │   │   └── Signup.tsx
│   │   ├── review/
│   │   │   ├── ExploreReviews.tsx
│   │   │   ├── ReviewForm.tsx
│   │   │   ├── ReviewList.tsx
│   │   │   └── ThankYou.tsx
│   │   └── user/
│   │       └── UserProfile.tsx
│   ├── contexts/
│   │   └── AuthContext.tsx
│   ├── firebase/
│   │   └── config.ts
│   ├── App.tsx
│   ├── index.css
│   └── main.tsx
├── .env
├── index.html
├── package.json
├── tsconfig.json
└── vite.config.ts
```

## Deployment

To deploy the application to Firebase Hosting:

1. Install Firebase CLI:
   ```bash
   npm install -g firebase-tools
   ```

2. Login to Firebase:
   ```bash
   firebase login
   ```

3. Initialize Firebase:
   ```bash
   firebase init
   ```
   Select Hosting and follow the prompts

4. Build the project:
   ```bash
   npm run build
   ```

5. Deploy to Firebase:
   ```bash
   firebase deploy
   ```

## Future Enhancements

- Add social login options (Google, Facebook)
- Implement review verification system
- Add seller response functionality
- Create a mobile app version
- Implement analytics for user behavior
- Add moderation for reviews

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.
