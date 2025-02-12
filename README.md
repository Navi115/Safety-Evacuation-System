# Safety-Evacuation-System
mkdir backend
cd backend
npm init -y
npm install express firebase-admin cors dotenv
serviceAccountKey.json
const admin = require('firebase-admin');
const serviceAccount = require('./serviceAccountKey.json');
admin.initializeApp({
  credential: admin.credential.cert(serviceAccount),
  databaseURL: "https://tu-proyecto.firebaseio.com"
});
