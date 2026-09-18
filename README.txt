MAILA'S GENERAL MERCHANDISE — V3 CLOUD INVENTORY

1) Open Supabase SQL Editor.
2) Paste and run supabase_setup.sql.
3) In Supabase Authentication, create an Email/Password user.
4) Upload this folder to Netlify (drag-and-drop the folder/zip).
5) Sign in using the Supabase user email/password.
6) Go to Inventory > Import Excel and select your RECORDS(2).xlsx.
   This imports the INVENTORY sheet into the shared cloud database.
7) Open the Netlify site on another browser/device and sign in with the same
   account. Inventory and sales will now come from the shared database.

IMPORTANT:
- The publishable/anon key is intended for frontend use when Row Level Security
  is correctly configured. Never put a Supabase service_role/secret key in this site.
- This version uses a 20% markup: selling price = SRP x 1.20.
- Sales are completed by a database function so stock deduction is atomic.
