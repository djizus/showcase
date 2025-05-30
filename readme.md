# Showcase

A community-driven showcase repository for projects. Add your project to be featured!

## How to Add Your Project

### 1. Fork this Repository

First, fork this repository to your GitHub account.

### 2. Add Your Project to `projects.json`

Edit the `projects.json` file and add your project entry. The file contains an array of project objects with the following structure:

```json
{
  "id": "your-project-id",
  "name": "Your Project Name",
  "description": "A brief description of your project (keep it concise but informative)",
  "category": "Category",
  "github": "https://github.com/your-username/your-repo",
  "website": "https://your-project-website.com",
  "twitter": "https://twitter.com/your-handle",
  "discord": "https://discord.gg/your-invite",
  "image": "https://raw.githubusercontent.com/[your-github-username]/showcase/main/images/[your-project-id]/[image-name].png",
  "featured": false
}
```

#### Field Descriptions:

- **id** (required): A unique identifier for your project (lowercase, no spaces, use hyphens)
- **name** (required): The display name of your project
- **description** (required): A brief description of what your project does
- **category** (required): The category your project belongs to (e.g., "Gaming", "DeFi", "Infrastructure", "Social", etc.)
- **github** (optional): Link to your project's GitHub repository
- **website** (optional): Your project's main website
- **twitter** (optional): Your project's Twitter/X profile
- **discord** (optional): Invite link to your project's Discord server
- **image** (required): URL to your project's showcase image (see image instructions below)
- **featured** (optional): Boolean value, typically set to `false` for new submissions

### 3. Add Your Project Image

1. Create a new directory in the `images/` folder with your project's ID:

   ```
   images/
     └── your-project-id/
   ```

2. Add your showcase image to this directory. Requirements:

   - **Format**: PNG or JPG
   - **Recommended dimensions**: 1200x630px (16:9 aspect ratio)
   - **File size**: Keep under 1MB for optimal loading
   - **Naming**: Use descriptive names (e.g., `showcase.png`, `your-project-name.png`)

3. Reference your image in the `projects.json` using the GitHub raw content URL format:

   ```
   https://raw.githubusercontent.com/[your-github-username]/showcase/main/images/[your-project-id]/[image-name].png
   ```

   Note: Replace `[your-github-username]` with your GitHub username after forking.

### 4. Submit a Pull Request

Once you've added your project to `projects.json` and added your image:

1. Commit your changes with a descriptive message:

   ```
   git add .
   git commit -m "Add [Your Project Name] to showcase"
   ```

2. Push to your fork and create a pull request to the main repository

## Example Entry

Here's a complete example of a project entry:

```json
{
  "id": "eternum",
  "name": "Realms: Eternum",
  "description": "Autonomous agents competing in a real-time onchain strategy game. Build your empire, manage resources, and conquer territories with AI-powered decision making.",
  "category": "Gaming",
  "github": "https://github.com/bibliothecadao/eternum",
  "website": "https://eternum.realms.world",
  "twitter": "https://twitter.com/realmseternum",
  "discord": "https://discord.gg/realmsworld",
  "image": "https://raw.githubusercontent.com/daydreamsai/showcase/main/images/eternum/eternum.png",
  "featured": true
}
```

## Guidelines

- **Be Accurate**: Ensure all information about your project is current and accurate
- **Quality Images**: Use high-quality images that represent your project well
- **Appropriate Content**: Only submit legitimate projects with appropriate content
- **No Duplicates**: Check that your project hasn't already been added
- **Keep it Updated**: If your project details change, submit a PR to update your entry

## Need Help?

If you have questions or run into issues:

1. Check existing entries in `projects.json` for reference
2. Ensure your JSON syntax is valid (you can use a JSON validator)
3. Make sure image paths are correctly referenced
4. Open an issue if you need assistance

---

Happy showcasing! 🚀
