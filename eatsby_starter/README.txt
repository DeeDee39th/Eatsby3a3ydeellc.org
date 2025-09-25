Eats By 3a3y Dee LLC — multi-site starter

Structure:
/site   -> main website (booking form + Stripe link)
/admin  -> private admin dashboard (protect with password in Netlify)
/jobs   -> employee job board (applications via Netlify Forms)

How to deploy in Netlify (create three sites, all from this repo):
- Main site: Base directory = site, Build command = (blank), Publish directory = .
- Admin site: Base directory = admin, Build command = (blank), Publish directory = .
- Jobs site: Base directory = jobs, Build command = (blank), Publish directory = .

Stripe:
- Replace the placeholder link in /site/index.html (search for 'REPLACE_THIS') with your Stripe Payment Link.

Email notifications:
- Netlify Dashboard -> Site -> Forms -> click each form -> Notifications -> add your email.
  Forms: booking (site), admin-create-job & employee-verify (admin), job-application (jobs).

Optional next steps:
- Add password to the Admin site (Netlify -> Site settings -> Site protection -> Password)
- Migrate jobs/applications to a database (Airtable/Google Sheets) using Netlify Functions.
