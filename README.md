# CampusCare — College Complaint & Resolution System

A colourful full-stack college complaint platform with two strict roles:

- **Student:** registers/logs in, raises complaints, and tracks Dean solutions.
- **College Dean:** logs in, reviews student complaints, sends a solution, records root cause and preventive action. **The Dean cannot raise complaints.**

## Local setup

1. Install Node.js LTS and PostgreSQL.
2. Create a PostgreSQL database named `college_complaints`.
3. Copy `.env.example` to `.env` and set your PostgreSQL connection string.
4. In the project folder run:

```bash
npm install
npm start
```

5. Open `http://localhost:3000`.

## Demo flow

Student → Login → Raise complaint → Dean login → Review complaint → Enter solution/root cause/preventive action → Send solution → Student sees resolution.

## Important

Never upload `.env` to GitHub. The production deployment should use environment variables and a cloud PostgreSQL database.
