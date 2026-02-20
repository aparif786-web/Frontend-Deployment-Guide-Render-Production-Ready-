# Frontend-Deployment-Guide-Render-Production-Ready-
https://your-backend-name.onrender.com
अच्छा 👍 अब बात साफ़ हो रही है।

आप कह रहे हो:

Backend Render server पर live है

Frontend को deploy करना है

Developer को clear command देनी है


ठीक है। मैं आपको बिल्कुल साफ़ निर्देश दे रहा हूँ, जो आप सीधे अपने developer को भेज सकते हो।


---

🚀 Frontend Deployment Guide (Render + Production Ready)

🔹 Step 1: Confirm Backend URL

Developer से बोलो:

Backend live URL confirm करो:

https://your-backend-name.onrender.com

Frontend में सभी API calls इस URL पर point करें।
Localhost हटाओ।


---

🔹 Step 2: Environment Variables Setup

अगर React / Next / Vite है तो:

.env.production file बनाओ:

VITE_API_URL=https://your-backend-name.onrender.com

Production build में यही use होना चाहिए।


---

🔹 Step 3: Build Command

Developer से बोलो:

npm run build

या अगर Flutter Web है:

flutter build web


---

🔹 Step 4: Deploy Frontend

Option A: Render Static Site

1. Render dashboard में जाओ


2. New → Static Site


3. GitHub repo connect करो


4. Build command:

npm install && npm run build


5. Publish directory:

dist

(या build depending on framework)




---

Option B: Vercel (Fastest for frontend)

GitHub connect करो

Auto deploy enable

Domain attach करो



---

🔹 Step 5: Domain + SSL

Custom domain add करो
SSL auto enable करो

Production domain example:

https://app.yourdomain.com


---

🔹 Step 6: Important Security Checks

Developer को बोलो:

CORS config backend में update करो

Only frontend domain allow करो

Rate limiting enable करो

JWT expiry check करो



---

⚠️ सबसे जरूरी

Render free plan पर अगर backend है:

Cold start issue होगा

15 मिनट inactivity पर sleep करेगा


अगर app serious है:

👉 Paid instance लो
👉 Auto scaling enable करो


---

🎯 Developer को यह exact message भेज सकते हो:

> Backend Render पर live है।
Frontend production build करो।
API URL production में update करो।
Static site Render/Vercel पर deploy करो।
CORS secure करो।
SSL enable करो।
Final QA test करो।




---

अब एक चीज़ clear करो:

Frontend किस technology में है?

1️⃣ React
2️⃣ Next.js
3️⃣ Flutter
4️⃣ Plain HTML/CSS
5️⃣ Other

