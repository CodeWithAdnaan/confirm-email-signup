# Email Confirmation Page

This is a simple standalone page used after Supabase email verification.
I kept everything in a single file (HTML, CSS, and JS together) so it can be deployed anywhere without any build process or extra setup.

## What this page does

* Shows a clear “Email Confirmed” message
* Automatically redirects the user to the login page after 5 seconds
* Also provides a manual “Go to Login” button
* Works directly with Supabase auth verification flow
* Includes Webryx credit with a clickable link

## Structure

Only one file is used:

email-confirmed.html

All design and logic are inside this file, no external dependencies.

## How to use

### 1. Set your login URL

Open the file and update this line:

const LOGIN_URL = "[https://your-main-site.com/login](https://your-main-site.com/login)";

Replace it with your actual website login link.

### 2. Deploy the file

You can host this page on any platform:

* Netlify
* Vercel
* GitHub Pages
* Any normal hosting

After deployment the URL will look like:

[https://confirm.yoursite.com](https://confirm.yoursite.com)

### 3. Connect with Supabase

Go to Supabase Dashboard → Authentication settings
and set the redirect URL to the place where this page is hosted:

[https://confirm.yoursite.com](https://confirm.yoursite.com)

After that, users who click the verification email will land on this page.

## User flow

1. User signs up
2. Verification email is sent
3. User clicks the link
4. This page opens
5. User is redirected to login automatically

## Customization

You can easily change:

* Text on the page
* Colors and style
* Redirect timing
* Add your logo on top

## Credits

Powered by Webryx.in
[https://webryx.in/](https://webryx.in/)
