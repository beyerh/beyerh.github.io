# Password Protection for Digital Garden

Your Digital Garden now has password protection that works with GitHub Pages!

## How It Works

- **Client-side protection**: Uses JavaScript to show a password prompt
- **Session-based**: Users stay logged in for the browser session
- **All pages protected**: Both the homepage and individual notes are protected

## Setup

1. **Set your password** in `.env`:
   ```bash
   SITE_PASSWORD=your_secure_password_here
   ```

2. **Build and deploy**:
   ```bash
   npm run build
   git add .
   git commit -m "Add password protection"
   git push
   ```

## Security Notes

⚠️ **This is basic protection** - not suitable for highly sensitive content:

- ✅ Prevents casual browsing
- ✅ Works with GitHub Pages (static hosting)
- ❌ Can be bypassed by technically skilled users
- ❌ Password is visible in page source (but obfuscated)

## How to Disable

To remove password protection, set an empty password in `.env`:
```bash
SITE_PASSWORD=
```

Then rebuild and redeploy your site.

## Customization

You can customize the login screen by editing:
`src/site/_includes/components/password-protection.njk`

## Testing

- Test locally: `npm start` and visit `http://localhost:8080`
- Current password: `test123`
- Correct password: `test123`

The site will show a login prompt. After entering the correct password, you'll have access to all pages during that browser session.
