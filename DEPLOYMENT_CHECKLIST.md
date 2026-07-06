# Deployment Checklist for Vibe Sharing

## Pre-Deployment Verification

- [x] Production build completed successfully
- [x] All files copied to deployment folder
- [x] README.md created with instructions
- [ ] Vibe Sharing access confirmed

## Vibe Sharing Deployment Steps

### Step 1: Access Vibe
- [ ] Log into Vibe Sharing platform
- [ ] Navigate to projects/folders section

### Step 2: Create Folder
- [ ] Click "New Folder" or "Create Project"
- [ ] Enter name: **"Staff Homepage"**
- [ ] Enter description: "Staff homepage prototype with approval/questionnaire cards and meeting flow v2"
- [ ] Set visibility/permissions as needed

### Step 3: Upload Files
- [ ] Upload `index.html`
- [ ] Upload `assets/` folder (entire folder)
- [ ] Upload `boardroom-pages/` folder
- [ ] Upload `doc-pages/` folder
- [ ] Upload all SVG files:
  - [ ] approval.svg
  - [ ] questionnaire.svg
  - [ ] atlas-logo.svg
  - [ ] diligent-d.svg
  - [ ] director-hp-card.svg
  - [ ] insights-empty-state.svg

### Step 4: Configure
- [ ] Verify all files uploaded successfully
- [ ] Check folder structure is preserved
- [ ] Set appropriate access permissions
- [ ] Note the deployed URL

### Step 5: Testing
- [ ] Open deployed URL
- [ ] Test password gate (if applicable)
- [ ] Test Approvals tab:
  - [ ] Click expand chevron on approval card
  - [ ] Verify approval progress shows
  - [ ] Check avatar badges display
  - [ ] Verify action buttons present
- [ ] Test Questionnaires tab:
  - [ ] Switch to Questionnaires tab
  - [ ] Expand questionnaire card
  - [ ] Verify submission progress shows
  - [ ] Check all action buttons present
- [ ] Test Meeting Flow:
  - [ ] Verify list view displays by default
  - [ ] Click stage filters (Planning, Pre-meeting, etc.)
  - [ ] Verify filtering works
  - [ ] Check meeting cards show metadata
- [ ] Test View Toggle:
  - [ ] Locate toggle at bottom-left
  - [ ] Click kanban view button
  - [ ] Verify kanban columns display
  - [ ] Click list view button
  - [ ] Verify returns to list view

### Step 6: Documentation
- [ ] Share deployed URL with team
- [ ] Document any access credentials
- [ ] Note deployment date and version
- [ ] Create announcement/notification if needed

## Post-Deployment

- [ ] Monitor for any issues
- [ ] Collect user feedback
- [ ] Document any bugs or enhancement requests

## Rollback Plan

If issues occur:
1. Take note of the issue
2. Remove deployment from Vibe
3. Fix issues in source
4. Rebuild: `npm run build`
5. Re-deploy following this checklist

## Contact Information

**Deployed By**: [Your Name]
**Deployment Date**: [Date]
**Deployed URL**: [URL after deployment]
**Version**: 1.0.0

## Notes

_Add any deployment-specific notes here_
