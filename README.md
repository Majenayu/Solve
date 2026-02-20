# PlacementPro – Integrated Campus Career Suite

Full-stack placement management dashboard for engineering colleges.

## Files
```
index.html   ← entire frontend (SPA)
server.js    ← entire backend (Express + all routes + all models)
package.json
.env         ← add your MONGO_URI here
render.yaml  ← Render deploy config
```

## Login
| Role    | Username | Password    |
|---------|----------|-------------|
| Admin   | `a`      | `a`         |
| Student | USN      | `student123`|

## Run Locally
```bash
npm install
node server.js
# Open http://localhost:3000
```

## CSV Import Format
```
Name,USN,Branch,Year,CGPA,Backlogs,Email,Phone
Rahul Sharma,1MS21CS001,CSE,4,8.5,0,rahul@example.com,9876543210
```

## Deploy on Render
1. Push to GitHub
2. New Web Service → connect repo
3. Build: `npm install` · Start: `node server.js`
4. Env var: `MONGO_URI` = your MongoDB connection string
