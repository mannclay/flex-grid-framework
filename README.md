# Flexgrid Layout Framework

The `.flexgrid` class functions as a container for flex items. It plays two roles: `.container` and `.row` classes as used in Bootstrap. You can also nest containers. To do so, use `.flexgrid-nm`, which removes the margin used for a parent container (e.g., wrapper for main content and sidebars).

## Grid System

### Default Breakpoints
Our grid system has five default breakpoints based on a twelve-column layout:

- **Extra extra large**: `col-xxl-`
- **Extra large**: `col-xl-`
- **Large**: `col-l-`
- **Medium**: `col-md-`
- **Small**: `col-sm-`

### Customization
Breakpoints, gutters, and margins are all customizable in the variables SCSS file.

### Column Spanning
Adding a number between `1-12` tells the class how many columns to span:

- `(col-xxl-9)` spans nine columns
- `(col-l-6)` spans six columns
- `(col-md-2)` spans two columns

---

## Example Layouts

### Basic Layout

#### Main Content and Sidebar
```html
<div class="col-xxl-9">
  <div>Main Content</div>
</div>
<div class="col-xxl-3">
  <div>Sidebar</div>
</div>

#### Two Columns
<div class="flexgrid-nm">
  <div class="col-xxl-6 col-md-6">
    <div>Content</div>
  </div>
  <div class="col-xxl-6 col-md-6">
    <div>Content</div>
  </div>
</div>

#### Three Columns
<div class="flexgrid-nm">
  <div class="col-xxl-4 col-md-4">
    <div>Content</div>
  </div>
  <div class="col-xxl-4 col-md-4">
    <div>Content</div>
  </div>
  <div class="col-xxl-4 col-md-4">
    <div>Content</div>
  </div>
</div>

#### Four Columns
<div class="flexgrid-nm">
  <div class="col-xxl-3 col-md-6">
    <div>Content</div>
  </div>
  <div class="col-xxl-3 col-md-6">
    <div>Content</div>
  </div>
  <div class="col-xxl-3 col-md-6">
    <div>Content</div>
  </div>
  <div class="col-xxl-3 col-md-6">
    <div>Content</div>
  </div>
</div>

