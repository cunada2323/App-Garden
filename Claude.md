# App-Garden

## Project Overview

App-Garden is a collection of web applications built with vanilla HTML, CSS, and JavaScript. The project serves as "Sunny's App Garden" - a repository of standalone web tools and applications.

## Project Structure

```
App-Garden/
├── index.html              # Landing page for the app collection
├── medication-tracker.html # Medication tracking application
└── Claude.md              # This file
```

## Tech Stack

- **Frontend**: Vanilla HTML5, CSS3, JavaScript (ES6+)
- **Storage**: LocalStorage for client-side data persistence
- **No build system**: Direct HTML files that can be opened in browsers
- **No dependencies**: Self-contained applications with no external libraries

## Applications

### 1. Index (index.html)
The main landing page that introduces the app collection.

### 2. Medication Tracker (medication-tracker.html)
A comprehensive medication tracking application with:
- Daily medication scheduling (Morning, Noon, Evening, Night)
- Medication management (add, edit, delete)
- Progress tracking and statistics
- History view for past medications
- Settings for customization
- Local storage persistence

## Development Guidelines

### Code Style
- Use semantic HTML5 elements
- Follow modern CSS practices (Flexbox, Grid)
- Use vanilla JavaScript (no frameworks)
- Keep applications self-contained in single HTML files
- Include all CSS in `<style>` tags
- Include all JavaScript in `<script>` tags

### File Naming
- Use lowercase with hyphens for file names: `medication-tracker.html`
- Keep descriptive, clear names

### Application Structure
Each application should be structured as:
1. HTML structure
2. CSS styles (in `<style>` tags)
3. JavaScript logic (in `<script>` tags)
4. Use LocalStorage for data persistence when needed

### Color Scheme
- Primary: #4A9B9B (teal/cyan)
- Background: #f5f5f5 (light gray)
- Text: #333 (dark gray)
- Cards/Containers: white with shadows

## Git Workflow

### Branch Naming
- Feature branches: `claude/create-<feature>-<session-id>`
- Development branch: `claude/create-claude-md-8uJIi`

### Commit Messages
- Use clear, descriptive commit messages
- Examples: "V2.3", "Adding medication tracker html", "Delete Med tracker.html.txt"

## Testing

### Manual Testing
- Test in multiple browsers (Chrome, Firefox, Safari, Edge)
- Test responsive design on mobile devices
- Verify LocalStorage functionality
- Test all interactive features

### Things to Check
- Does the app work offline?
- Is data persisted correctly in LocalStorage?
- Are all buttons and interactions working?
- Is the UI responsive on mobile?
- Are there any console errors?

## Common Tasks

### Adding a New Application
1. Create a new HTML file: `app-name.html`
2. Include complete HTML structure with embedded CSS and JS
3. Update `index.html` to link to the new app
4. Test thoroughly in multiple browsers
5. Commit with descriptive message

### Modifying Existing Applications
1. Read the entire file to understand the structure
2. Locate the relevant section (HTML, CSS, or JS)
3. Make focused changes without over-engineering
4. Test the changes thoroughly
5. Commit with clear message

### Working with LocalStorage
- Each app uses its own LocalStorage keys
- Example: `medicationSchedule`, `medications`, etc.
- Always handle cases where data might not exist
- Consider data migration if changing storage format

## Known Patterns

### Application Template
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>App Name</title>
    <style>
        /* Styles here */
    </style>
</head>
<body>
    <!-- HTML structure here -->
    <script>
        // JavaScript here
    </script>
</body>
</html>
```

### LocalStorage Pattern
```javascript
// Save data
localStorage.setItem('key', JSON.stringify(data));

// Load data
const data = JSON.parse(localStorage.getItem('key') || '{}');
```

## Troubleshooting

### LocalStorage Issues
- Check if localStorage is available in the browser
- Verify data is being saved correctly with browser DevTools
- Clear localStorage if data becomes corrupted

### Styling Issues
- Check browser compatibility for CSS features
- Verify responsive design with DevTools device emulation
- Test hover states and interactions

## Future Considerations

- Consider adding a proper navigation system in index.html
- May want to add service worker for offline functionality
- Could add export/import functionality for data backup
- Consider adding PWA manifest for installability

## Resources

- Repository: cunada2323/App-Garden
- No external documentation or dependencies
- All code is self-contained in HTML files
