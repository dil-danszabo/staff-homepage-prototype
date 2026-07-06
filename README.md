# Staff Homepage - Vibe Sharing Deployment

## Overview
This folder contains the production build of the Staff Homepage prototype with the following features:

### Features Implemented
- ✅ **Expanded Approval Cards** with detailed progress tracking
  - Progress ring visualization
  - Status breakdown (Approved, Rejected, Abstained, Not responded)
  - Avatar badges for respondents
  - Action buttons (Remind participants, Open details)

- ✅ **Expanded Questionnaire Cards** with submission progress
  - Submission progress tracking
  - Status breakdown (Submitted, In Progress, Unopened)
  - Action buttons (Remind participants, Change close date, Close survey)

- ✅ **Dynamic Icons**
  - Approval cards: approval.svg (bell icon)
  - Questionnaire cards: questionnaire.svg (document with magnifying glass)

- ✅ **Meeting Flow V2**
  - Sidebar with stage filters (Planning, Pre-meeting, In Meeting, Post meeting)
  - List view with detailed metadata (topics, presenters, hours allocated)
  - Clickable stage filters with counts

- ✅ **View Toggle**
  - Subtle toggle button at bottom-left of sidebar
  - Switch between Kanban view (columns) and List view (sidebar + list)
  - Active state highlighting

### Tab Functionality
- **Approvals Tab**: Shows 4 approval items with expand/collapse
- **Questionnaires Tab**: Shows 4 questionnaire items with expand/collapse

## Deployment Instructions

### To Vibe Sharing:

1. **Access Vibe Sharing Platform**
   - Navigate to the Vibe sharing interface
   - Look for "New Folder" or "Create Project" option

2. **Create New Folder**
   - Name: "Staff Homepage"
   - Description: "Staff homepage prototype with approval/questionnaire cards and meeting flow"

3. **Upload Files**
   - Upload all contents of this folder to the "Staff Homepage" folder
   - Ensure the folder structure is preserved:
     - `index.html` (root)
     - `assets/` folder
     - `boardroom-pages/` folder
     - `doc-pages/` folder
     - SVG files (approval.svg, questionnaire.svg, etc.)

4. **Verify Deployment**
   - Access the deployed URL
   - Check that all features work:
     - Approval cards expand/collapse
     - Questionnaire cards expand/collapse
     - Meeting flow view toggle works
     - Tab switching works

### Alternative: Netlify Deployment

If deploying to Netlify instead:

```bash
# Install Netlify CLI if not already installed
npm install -g netlify-cli

# Deploy
cd /Users/danszabo/Desktop/staffHomeP/Staff_homepage_deploy
netlify deploy --prod

# Follow the prompts to authorize and select/create a site
```

## Technical Details

- **Framework**: React 19 + Vite
- **UI Library**: Material-UI (MUI) + Diligent Atlas React Bundle
- **Build Size**: ~3.2 MB (JS), ~372 KB (CSS)
- **Browser Support**: Modern browsers (Chrome, Firefox, Safari, Edge)

## Files Structure

```
Staff_homepage_deploy/
├── index.html              # Entry point
├── assets/                 # JS, CSS, fonts
├── boardroom-pages/        # Additional pages
├── doc-pages/             # Documentation pages
├── approval.svg           # Approval icon
├── questionnaire.svg      # Questionnaire icon
├── atlas-logo.svg         # Atlas logo
├── diligent-d.svg         # Diligent logo
└── insights-empty-state.svg
```

## Notes

- The app includes a password gate for prototype protection
- Default password hash is stored in the bundle (client-side only)
- All interactions are client-side only (no backend required)
- The app is fully responsive and works on desktop/tablet

## Support

For questions or issues with deployment, contact the development team.

---

**Built**: July 6, 2026
**Version**: 1.0.0
