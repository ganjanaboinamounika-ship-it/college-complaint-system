# Windows local setup

## 1. PostgreSQL
Create a database called `college_complaints` in pgAdmin.

## 2. Environment
Create `.env` in the project root:

```env
DATABASE_URL=postgresql://postgres:YOUR_PASSWORD@localhost:5432/college_complaints
SESSION_SECRET=replace-with-a-long-random-secret
DEAN_ACCESS_CODE=DEAN-2026
NODE_ENV=development
PORT=3000
```

## 3. Install and run

```powershell
npm install
npm start
```

Open `http://localhost:3000`.

## 4. Test roles

Student account: create a student account and submit a complaint.

Dean account: create a Dean account using `DEAN-2026`. The Dean dashboard contains **no complaint submission form**. The Dean can only review student complaints and send solutions.
