# Build Your Personal Website with Claude Code

A step-by-step guide to creating and deploying your own website using Claude Code and GitHub Pages.

---

## What You'll End Up With

- A personal website live on the internet at `https://yourusername.github.io`
- Complete control over the design and content
- Free hosting that updates automatically when you make changes

---

## Before You Start

Make sure you have these ready:

### 1. GitHub Account
You already have this! Make sure you know your username and password.

### 2. Node.js (Required for building websites)

Check if you have it by opening Terminal and typing:
```bash
node --version
```

If you see a version number (like `v20.10.0`), you're good! If not, install it:
1. Go to https://nodejs.org
2. Download the **LTS** version (the one that says "Recommended")
3. Run the installer and follow the prompts
4. Restart Terminal and check again with `node --version`

### 3. Git (For saving and publishing your code)

Check if you have it:
```bash
git --version
```

If not installed, macOS will prompt you to install it. Follow the prompts.

### 4. Claude Code

If you don't have Claude Code installed yet:
```bash
npm install -g @anthropic-ai/claude-code
```

Then log in:
```bash
claude login
```

---

## Step 1: Create Your GitHub Repository

This is where your website code will live. The repository name determines your website URL.

1. Go to https://github.com/new
2. For **Repository name**, enter exactly: `yourusername.github.io`
   - Replace `yourusername` with your actual GitHub username
   - Example: if your username is `jane-doe`, the repo name is `jane-doe.github.io`
3. Make sure **Public** is selected (required for free GitHub Pages)
4. Check the box for **Add a README file**
5. Click **Create repository**

Your website URL will be: `https://yourusername.github.io`

---

## Step 2: Clone the Repository to Your Computer

1. Open Terminal
2. Navigate to where you want to keep your projects:
   ```bash
   cd ~/Documents
   ```
   (or wherever you prefer)

3. Clone your new repository:
   ```bash
   git clone https://github.com/yourusername/yourusername.github.io.git
   ```

4. Enter the project folder:
   ```bash
   cd yourusername.github.io
   ```

---

## Step 3: Start Claude Code

Now the fun part begins! Start Claude Code in your project folder:

```bash
claude
```

---

## Step 4: Tell Claude What You Want

This is where you get creative! Claude will help you design and build your website based on what you describe. Here's how to start the conversation:

### Introduce Your Project

Start with something like:

> "I want to build a personal website that will be hosted at https://yourusername.github.io. Let's use Astro as the framework since it's great for static sites and works well with GitHub Pages."

### Describe Your Vision

Think about:
- **Purpose**: What is this website for? Portfolio? Blog? Just a fun personal page?
- **Vibe**: What feeling do you want? Modern? Cozy? Minimalist? Colorful? Dark mode?
- **Content**: What pages do you want? What will you put on them?
- **Inspiration**: Any websites you love the look of?

Example prompts to get you started:

> "I want a portfolio website to showcase my art and photography. I'm thinking a clean, minimal design with lots of white space to let the images stand out. Maybe a light color scheme with one accent color."

> "I want a personal blog where I can write about my interests. I'd love a cozy, warm aesthetic - maybe earthy colors and a font that feels friendly. I want a home page, an about page, and a blog section."

> "I want a simple landing page about me - who I am, my interests, links to my social media. I want it to feel modern and cool, maybe with some subtle animations."

### Let Claude Guide You

Claude will probably ask you follow-up questions to understand your vision better. Answer them honestly! There are no wrong answers - this is YOUR website.

Claude might ask things like:
- What colors do you like?
- Do you want a dark or light theme?
- What pages do you need?
- Do you have images/photos to include?
- What's your name/brand name for the site?

---

## Step 5: Build Together

Claude will start creating your website. Here's what to expect:

### The Building Process

1. **Project Setup**: Claude will set up Astro and the basic project structure
2. **Design System**: Claude will create your color scheme, fonts, and overall look
3. **Pages**: Claude will build each page you discussed
4. **Components**: Claude will create reusable pieces like headers, footers, and cards
5. **Content**: You'll work together to add your actual content

### Preview Your Site

At any point, you can see your website locally. Ask Claude:

> "Can you start the dev server so I can preview the site?"

Claude will run:
```bash
npm run dev
```

Then open your browser to `http://localhost:4321` to see your site!

### Give Feedback

As you preview, tell Claude what you think:

> "I love the header! But can we make the accent color more blue instead of purple?"

> "The font feels too formal. Can we try something more casual?"

> "Can you add a section for my favorite quotes on the about page?"

> "This is perfect! Let's move on to the next page."

---

## Step 6: Add Your Content

Once the structure is ready, add your personal content:

### Text Content
Tell Claude what to put on each page:

> "On the about page, here's what I want to say: [your bio, interests, etc.]"

### Images
For images, you'll need to:
1. Put your image files in the `public/images/` folder
2. Tell Claude the filenames so it can add them to your pages

> "I added my profile photo as `public/images/me.jpg`. Can you add it to the about page?"

### Links
Share your social media links:

> "Here are my social links to add to the footer:
> - Instagram: https://instagram.com/yourhandle
> - GitHub: https://github.com/yourusername"

---

## Step 7: Set Up Automatic Deployment

This makes your site automatically update whenever you push changes to GitHub.

Ask Claude:

> "Can you set up the GitHub Actions workflow for deploying to GitHub Pages?"

Claude will create the necessary files. This only needs to be done once.

---

## Step 8: Publish Your Website

When you're happy with your site, it's time to go live!

Ask Claude:

> "I'm ready to publish! Can you commit all the changes and push to GitHub?"

Claude will:
1. Add all the files to git
2. Create a commit with a descriptive message
3. Push everything to GitHub

### Enable GitHub Pages

After the first push, you need to enable GitHub Pages (one-time setup):

1. Go to your repository on GitHub
2. Click **Settings** (top menu)
3. Click **Pages** (left sidebar)
4. Under **Source**, select **GitHub Actions**
5. Wait a few minutes for the first deployment

### See Your Live Site!

Visit `https://yourusername.github.io` - your website is live!

---

## Step 9: Making Updates Later

Whenever you want to update your site:

1. Open Terminal
2. Navigate to your project:
   ```bash
   cd ~/Documents/yourusername.github.io
   ```
3. Start Claude:
   ```bash
   claude
   ```
4. Tell Claude what you want to change:
   > "I want to add a new blog post about..."

   > "Can we change the accent color to..."

   > "I want to add a new page for..."

5. When done, ask Claude to push the changes:
   > "Push these changes to GitHub"

Your live site will update automatically in a few minutes!

---

## Tips for Working with Claude

### Be Specific
The more details you give, the better the result:
- Instead of "make it look nice" try "I want a minimalist look with lots of whitespace, a serif font for headings, and a soft sage green accent color"

### Iterate
You don't have to get everything perfect the first time:
- Start with a basic version
- Preview it
- Give feedback
- Refine step by step

### Save Your Progress
Ask Claude to commit periodically:
> "Let's commit what we have so far"

This saves your progress in case anything goes wrong.

### Ask Questions
If Claude suggests something you don't understand, ask!
> "What does that mean?"
> "Why did you choose that approach?"
> "Can you explain how this works?"

### Have Fun!
This is YOUR creative project. Experiment with ideas. Try things that might not work. You can always change it!

---

## Troubleshooting

### "Command not found: node"
Node.js isn't installed or Terminal needs to be restarted. See the Node.js installation steps above.

### "Command not found: claude"
Claude Code isn't installed. Run:
```bash
npm install -g @anthropic-ai/claude-code
```

### Site not updating after push
- Check that GitHub Pages is set to use "GitHub Actions" as the source
- Go to your repo's **Actions** tab to see if the build is running or failed
- Wait a few minutes - it can take time to deploy

### Preview not working
Make sure the dev server is running (`npm run dev`) and you're visiting the correct URL (usually `http://localhost:4321`)

---

## Ideas to Get You Started

Not sure what to put on your site? Here are some ideas:

### For a Portfolio
- Showcase your art, photography, writing, music, or other creative work
- Include an about page with your bio
- Add a contact page or social links

### For a Blog
- Write about your hobbies, interests, or things you're learning
- Share book reviews, movie thoughts, or game reviews
- Document a project or journey

### For a Personal Page
- Introduce yourself
- Share your interests and what makes you, you
- Link to your other online presence
- Include a fun "now" page about what you're currently into

### Fun Additions
- A page of your favorite quotes
- A list of recommendations (books, music, shows)
- A guestbook (requires more advanced setup)
- An "interests" or "things I love" page
- A page about your pets!

---

## You've Got This!

Building a website is a creative process. There's no single "right" way to do it. Work with Claude, experiment, and make something that feels like YOU.

Your website will be live at: **https://yourusername.github.io**

Happy building!
