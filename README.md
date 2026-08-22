# Wear Echoo — Vercel package

This package contains:
- store/index.html — customer storefront
- admin/index.html — admin dashboard
- vercel.json — Vercel routing config

IMPORTANT SECURITY/PRODUCTION NOTE:
The storefront uses the Supabase publishable key in browser code, which is normal only when database Row Level Security policies are correctly configured.

The current admin page uses the Supabase REST API with the publishable key but DOES NOT yet enforce Supabase Auth in the page itself. Before public launch, add Supabase Auth login/session checks to the admin and tighten policies as needed. Do not put a Supabase secret/service-role key in frontend code.

UPI:
wear-echo@ptyes

Deployment:
1. Upload this folder to a GitHub repository.
2. Import the repository into Vercel.
3. Deploy.
4. Store URL: your Vercel domain.
5. Admin URL: /admin/

For production, also configure image storage (Supabase Storage) and authenticated admin access.
