# Google AdSense + Vercel deployment steps

## Changes prepared
- Added the AdSense publisher script to every top-level HTML page.
- Added `ads.txt` for publisher ID `pub-8072233087398262`.
- Existing page layouts and site assets were otherwise left unchanged.

## Deploy to Vercel
1. Extract this ZIP on your computer.
2. Open the project folder `SML_Property_Management` and check that `index.html`, `about.html`, `services.html`, `contact.html`, `ads.txt`, `css/`, `js/`, and `image/` are present.
3. Commit and push the project to the Git repository connected to Vercel, or import the folder/repository into Vercel.
4. For this static HTML site, use the project root as the Root Directory. No build command is normally needed; set the Output Directory to `.` if Vercel asks for one. Do not add a framework preset unless the repository is configured for one.
5. Deploy, then open the production domain and verify each page loads.
6. Check `https://YOUR-DOMAIN/ads.txt` and confirm it displays: `google.com, pub-8072233087398262, DIRECT, f08c47fec0942fa0`.
7. In Google AdSense, add/verify the exact production domain, request review if needed, and enable Auto ads or create ad units. The script alone does not guarantee that ads will display; Google approval, site eligibility, consent requirements where applicable, and ad-serving decisions still apply.
8. After deployment, use AdSense's site status and policy pages to check for errors. Allow time for crawling and ad serving.

## Important
- The ZIP contains static website files. This update does not itself deploy to Vercel or change DNS.
- Do not share your Google account password or private credentials. The publisher ID is not a password.
