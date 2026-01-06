# Cleanup Plan - Unused Files Analysis
## Pre-Modernization Cleanup

**Goal**: Remove unused files and test to ensure site still works before beginning modernization.

---

## Step 1: Create Backup
**Status**: ⏳ Pending

- [ ] Create `index.html.backup` (copy of current index.html)
- [ ] Document backup creation date/time
- [ ] Verify backup file exists and is readable

---

## Step 2: Test Current Site Baseline
**Status**: ⏳ Pending

**Test Checklist**:
- [ ] Site loads without errors
- [ ] All 15 gallery images display
- [ ] Thumbnail navigation works
- [ ] Click main image advances to next
- [ ] Browser back button works
- [ ] Fade transitions work
- [ ] Thumbnail hover effects work
- [ ] Rounded corners on main container visible
- [ ] Drop shadow on h1 visible
- [ ] All CSS styles applied correctly
- [ ] No console errors
- [ ] No 404 errors in network tab

**Document Results**:
- Browser tested: ___________
- Date: ___________
- Issues found: ___________

---

## Step 3: Identify Unused Files

### Files Currently Used (DO NOT DELETE)

**CSS Files** (referenced in index.html):
- ✅ `css/reset.css`
- ✅ `css/text.css`
- ✅ `css/960.css`
- ✅ `css/style.css`
- ✅ `css/galleria.css`

**JavaScript Files** (referenced in index.html):
- ✅ `jquery-1.2.6.min.js`
- ✅ `jquery.galleria.js`
- ✅ `jquery.curvycorners.min.js` (used for `.corner()` method)
- ✅ `jquery.plugin.dropshadow.js` (used for `.dropShadow()` method)

**Images** (referenced in index.html):
- ✅ `images/1.jpg` through `images/15.jpg` (15 gallery images)
- ✅ `images/background.png` (referenced in CSS: `url(../images/background.png)`)

**Root Files**:
- ✅ `index.html` (main page)
- ✅ `background.png` (may be used, need to verify)

---

### Files Likely Unused (CANDIDATES FOR DELETION)

**Root Level Files**:
- ❓ `index.php` - Old/test version, not referenced
- ❓ `style.css` - Root level, not referenced (using `css/style.css` instead)
- ❓ `test.txt` - Test file
- ❓ `background.png` - Root level, may be duplicate of `images/background.png`

**JavaScript Files**:
- ❓ `galleria-1.2.9.js` - Not referenced (using `jquery.galleria.js` instead)
- ❓ `galleria-1.2.9.min.js` - Not referenced
- ❓ `jquery-1.9.1.min.js` - Not referenced (using 1.2.6)
- ❓ `jquery.corner.js` - Not referenced (using `jquery.curvycorners.min.js`)
- ❓ `jquery.galleria.pack.js` - Not referenced

**CSS Files**:
- ❓ `css/960.css.bak` - Backup file
- ❓ `css/galleria.classic.css` - Not referenced
- ❓ `css/uncompressed/` directory - Backup/uncompressed versions

**Images**:
- ❓ `images/1b.jpg` - Not in gallery list
- ❓ `images/1c.jpg` - Not in gallery list
- ❓ `images/old/` directory - Backup/archived images
- ❓ `images/Thumbs.db` - Windows thumbnail cache file

---

## Step 4: Verify Unused Files

**Before deleting, verify**:
- [ ] Check if `background.png` (root) is different from `images/background.png`
- [ ] Check if any CSS references root `background.png`
- [ ] Check if `images/1b.jpg` or `images/1c.jpg` are referenced anywhere
- [ ] Confirm `index.php` is not used in production
- [ ] Check if any external links point to `index.php`

---

## Step 5: Safe Deletion Plan

### Phase A: Definitely Safe to Delete (No Verification Needed)
- [ ] `test.txt` - Test file
- [ ] `images/Thumbs.db` - Windows system file
- [ ] `css/960.css.bak` - Backup file
- [ ] `css/uncompressed/` directory - Backup files

### Phase B: Verify Then Delete
- [ ] `index.php` - Verify not in production use
- [ ] `style.css` (root) - Verify not referenced
- [ ] `galleria-1.2.9.js` - Verify not referenced
- [ ] `galleria-1.2.9.min.js` - Verify not referenced
- [ ] `jquery-1.9.1.min.js` - Verify not referenced
- [ ] `jquery.corner.js` - Verify not referenced (different from curvycorners)
- [ ] `jquery.galleria.pack.js` - Verify not referenced
- [ ] `css/galleria.classic.css` - Verify not referenced
- [ ] `images/1b.jpg` - Verify not referenced
- [ ] `images/1c.jpg` - Verify not referenced
- [ ] `images/old/` directory - Verify not referenced
- [ ] `background.png` (root) - Verify if duplicate or unused

---

## Step 6: Execute Deletion

**Order of Operations**:
1. Delete Phase A files (definitely safe)
2. Test site again
3. If tests pass, delete Phase B files one at a time
4. Test after each deletion
5. Document what was deleted

---

## Step 7: Post-Cleanup Testing

**Test Checklist** (same as Step 2):
- [ ] Site loads without errors
- [ ] All 15 gallery images display
- [ ] Thumbnail navigation works
- [ ] Click main image advances to next
- [ ] Browser back button works
- [ ] Fade transitions work
- [ ] Thumbnail hover effects work
- [ ] Rounded corners on main container visible
- [ ] Drop shadow on h1 visible
- [ ] All CSS styles applied correctly
- [ ] No console errors
- [ ] No 404 errors in network tab

---

## Files to Delete (Final List)

### Safe to Delete Immediately:
```
test.txt
images/Thumbs.db
css/960.css.bak
css/uncompressed/ (entire directory)
```

### Verify Then Delete:
```
index.php
style.css (root level)
galleria-1.2.9.js
galleria-1.2.9.min.js
jquery-1.9.1.min.js
jquery.corner.js
jquery.galleria.pack.js
css/galleria.classic.css
images/1b.jpg
images/1c.jpg
images/old/ (entire directory)
background.png (root level - verify first)
```

---

## Notes

- **Never delete files that are referenced in index.html**
- **Always test after deletions**
- **Keep backups of everything before deleting**
- **Document what was deleted and why**

---

## Execution Log

**Date**: January 6, 2025

**Phase A Deletions**:
- [x] test.txt ✅ Deleted
- [x] images/Thumbs.db ✅ Deleted
- [x] css/960.css.bak ✅ Deleted
- [x] css/uncompressed/ ✅ Deleted

**Phase B Deletions**:
- [x] style.css (root level) ✅ Deleted - Not referenced, using css/style.css instead
- [x] background.png (root level) ✅ Deleted - Not referenced, using images/background.png
- [x] galleria-1.2.9.js ✅ Deleted - Not referenced, using jquery.galleria.js
- [x] galleria-1.2.9.min.js ✅ Deleted - Not referenced
- [x] jquery-1.9.1.min.js ✅ Deleted - Not referenced, using jquery-1.2.6.min.js
- [x] jquery.corner.js ✅ Deleted - Not referenced, using jquery.curvycorners.min.js
- [x] jquery.galleria.pack.js ✅ Deleted - Not referenced
- [x] css/galleria.classic.css ✅ Deleted - Not referenced
- [x] images/1b.jpg ✅ Deleted - Not in gallery
- [x] images/1c.jpg ✅ Deleted - Not in gallery
- [x] images/old/ ✅ Deleted - Backup directory

**Files Kept (Need Verification)**:
- [x] index.php ✅ Deleted - Confirmed unused: broken references, placeholder content, duplicate head tags

**Post-Cleanup Test Results**:
- [ ] All tests passed - **PENDING: User needs to test site**
- [ ] Site fully functional - **PENDING: User needs to test site**

**Issues Found**:
- None so far - awaiting user testing confirmation

