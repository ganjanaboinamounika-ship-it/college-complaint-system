# Deployment and Custom Domain

## Render
1. Create a Render PostgreSQL database.
2. Create a Render Web Service from this GitHub repository.
3. Build command: `npm install`
4. Start command: `npm start`
5. Add environment variables:
   - NODE_ENV=production
   - DATABASE_URL=<Render PostgreSQL connection string>
   - SESSION_SECRET=<long random secret>
   - DEAN_ACCESS_CODE=<private code>
6. Deploy and test the generated Render URL.
7. In the service's Custom Domains area, add `collegecomplaintsystem.in`.
8. Add the DNS records Render provides at your domain registrar.
9. Wait for verification and HTTPS.
10. Test `https://collegecomplaintsystem.in`.

Never upload `.env` to GitHub. Change the dean access code before public use.
