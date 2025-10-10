# Reports Folder

This folder contains visual reports, dashboards, and analysis outputs for the Bellabeat Case Study project.

## How to Import JPG Files to This Folder

There are several ways to add JPG (or other image) files to this reports folder:

### Method 1: Using Git Command Line

1. Save your JPG file to your local computer
2. Navigate to your local repository clone:
   ```bash
   cd /path/to/google-data-analytics-bellabeat-casestudy
   ```
3. Copy your JPG file to the reports folder:
   ```bash
   cp /path/to/your/image.jpg reports/
   ```
4. Add the file to git:
   ```bash
   git add reports/image.jpg
   ```
5. Commit the changes:
   ```bash
   git commit -m "Add report image"
   ```
6. Push to GitHub:
   ```bash
   git push origin main
   ```

### Method 2: Using GitHub Web Interface

1. Go to the repository on GitHub: `https://github.com/Vwnsk/google-data-analytics-bellabeat-casestudy`
2. Navigate to the `reports` folder
3. Click on "Add file" → "Upload files"
4. Drag and drop your JPG files or click "choose your files"
5. Add a commit message describing the files
6. Click "Commit changes"

### Method 3: Using GitHub Desktop (if you use it)

1. Open GitHub Desktop
2. Select this repository
3. Copy your JPG files to the `reports` folder in your local repository
4. GitHub Desktop will detect the changes
5. Add a commit message and commit
6. Click "Push origin" to upload to GitHub

## Recommended File Naming Convention

For better organization, use descriptive names for your images:
- `looker_dashboard.jpg` - Main Looker Studio dashboard
- `activity_analysis.jpg` - Activity analysis charts
- `sleep_patterns.jpg` - Sleep pattern visualizations
- `correlation_steps_calories.jpg` - Steps vs Calories scatter plot
- etc.

## Supported Image Formats

You can add the following image formats:
- JPG/JPEG (`.jpg`, `.jpeg`)
- PNG (`.png`)
- GIF (`.gif`)
- SVG (`.svg`)

## Referencing Images in README

Once you've uploaded an image to the reports folder, you can reference it in the main README.md using relative paths:

```markdown
![Dashboard](reports/looker_dashboard.jpg)
```

Or using HTML for more control:

```html
<img src="reports/looker_dashboard.jpg" alt="Looker Dashboard" width="800">
```

## Current Reports

- Add your report files here following the instructions above
