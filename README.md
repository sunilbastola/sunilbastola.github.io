## Personal Portfolio Website

A modern, responsive personal portfolio built as a static site (no build step). It highlights my skills, projects, research interests, and includes a contact section.

### Tools Used

- **HTML**: Page structure (`index.html`)
- **CSS**: Styling + responsive layout (`style.css`)
- **GitHub**: Version control + hosting (GitHub Pages)
- **Font Awesome**: Icons
- **Google Fonts**: Typography (Poppins, Raleway)

### Features

- **Modern card-based layout** (Skills / Projects / Education / Leadership / References)
- **Research & Model Building section** for AI-focused profile
- **Responsive navigation** with mobile menu toggle
- **Hero headshot** with circular crop + accent ring
- **Projects** linked directly to GitHub repositories
- **Contact section** with quick links (email, LinkedIn, website)

### Project Structure

- **`index.html`**: Main page content
- **`style.css`**: Styling and responsive rules
- **`assets/`**: Static files (e.g., headshot image)
  - **`assets/headshot.jpg`**: Hero image

### Run Locally

Because this is a static site, you can open the file directly:

- Open `index.html` in your browser

For best results (relative paths + consistent behavior), run a local server:

```bash
cd portfolio-website
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

### Customize

- **Profile photo**: Replace `assets/headshot.jpg` with your preferred photo (keep the same filename for zero code changes).
- **Hero text**: Update the headline and summary in `index.html` inside the `section.hero`.
- **Projects**: Edit the cards in `index.html` under `section#projects` (update names, descriptions, and GitHub links).
- **Links**: Update social/contact links near the top of `index.html` (email, LinkedIn, GitHub, website).

### Deploy to GitHub Pages

1. Push this repository to GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose:
   - **Source**: “Deploy from a branch”
   - **Branch**: `main` (or `master`) and `/root`
4. Save — GitHub will publish your site and show the URL.

### Contact Form (Optional)

The form is currently static. To make it “send messages”, you can:

- **Use a form service** (fastest): Formspree / Getform / Basin  
- **Use serverless** (recommended): Netlify/Vercel/Cloudflare Functions + an email provider (SendGrid/Mailgun/SES/Resend)
- **Use your own backend**: e.g., FastAPI endpoint + email provider

### Credits

- Icons: Font Awesome
- Fonts: Google Fonts


