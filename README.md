# Zen Z ka Dukan
Black-and-gold mobile-first fashion store starter using React, Vite and Supabase.

## GitHub
Upload the contents of this folder to a new GitHub repository (not the ZIP itself). On Android, extract the ZIP first, then upload files using GitHub's website or a supported Git client.

## Supabase setup
1. Create a Supabase project.
2. In SQL Editor run `supabase/schema.sql`.
3. Create `.env` based on `.env.example` and add Project URL + anon/public key (never service-role key).
4. Enable Email/Password under Authentication.
5. Sign up in the app, then run the admin promotion SQL at the bottom of schema.sql with your email.
6. Add product rows using Admin. This starter's admin form supports image URLs, not direct file upload yet.
7. Deploy the repository to a compatible static host and add the same environment variables in its settings.

## Important
This is a starter project, not a fully production-hardened store. Before accepting real orders, implement server-side order creation that calculates prices from the database and atomically validates/decrements colour-size stock. Current browser-side order insertion is not enough for production. Configure storage upload policies before enabling image upload. Mobile OTP is not implemented; this version uses email/password. Free hosting/AI limits can change.
