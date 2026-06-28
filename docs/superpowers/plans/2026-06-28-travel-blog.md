# Travel Blog Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Build a GitHub Pages-ready Jekyll travel blog with a magazine-style homepage, six requested categories, sample articles, and clear photo instructions.

**Architecture:** The site uses Jekyll layouts and includes to render Markdown posts into static HTML on GitHub Pages. Data for categories lives in `_data/categories.yml`, page layout lives in `_layouts/`, and presentation lives in `assets/css/style.css`.

**Tech Stack:** Jekyll, GitHub Pages, Markdown, HTML, CSS.

---

## File Structure

- Create `_config.yml` for Jekyll metadata and permalink settings.
- Create `_data/categories.yml` for the six category definitions.
- Create `_layouts/default.html`, `_layouts/home.html`, `_layouts/post.html`, and `_layouts/category.html`.
- Create `index.md`, `about.md`, and one category page per requested category.
- Create six sample posts in `_posts/`.
- Create `assets/css/style.css` for the magazine layout.
- Create `assets/images/README.md` explaining photo placement.
- Create `README.md` with local editing and GitHub Pages publishing steps.

### Task 1: Project Shell

**Files:**
- Create: `.gitignore`
- Create: `_config.yml`
- Create: `_data/categories.yml`
- Create: `README.md`
- Create: `assets/images/README.md`

- [ ] **Step 1: Create project configuration**

Create the files listed above with Jekyll settings, category metadata, photo folder instructions, and publishing instructions.

- [ ] **Step 2: Verify static structure**

Run: `find . -maxdepth 3 -type f | sort`
Expected: the config, data, README, and image README files are present.

- [ ] **Step 3: Commit**

Run: `git add . && git commit -m "chore: add travel blog project shell"`

### Task 2: Layouts And Styles

**Files:**
- Create: `_layouts/default.html`
- Create: `_layouts/home.html`
- Create: `_layouts/post.html`
- Create: `_layouts/category.html`
- Create: `assets/css/style.css`

- [ ] **Step 1: Create Jekyll layouts**

Create default navigation, homepage, post, and category layouts. Layouts must render categories from `_data/categories.yml` and posts from `site.posts`.

- [ ] **Step 2: Create magazine styling**

Create a responsive editorial layout with a large hero story, compact story cards, readable article pages, and category chips.

- [ ] **Step 3: Verify required Liquid tags**

Run: `rg "site.posts|site.data.categories|page.category|content" _layouts`
Expected: all key rendering hooks are present.

- [ ] **Step 4: Commit**

Run: `git add _layouts assets/css/style.css && git commit -m "feat: add magazine layouts and styles"`

### Task 3: Pages And Sample Stories

**Files:**
- Create: `index.md`
- Create: `about.md`
- Create: `categories/uzbekistan.md`
- Create: `categories/hungary.md`
- Create: `categories/cote-d-azur.md`
- Create: `categories/japan.md`
- Create: `categories/food.md`
- Create: `categories/stays.md`
- Create: six files in `_posts/`

- [ ] **Step 1: Create pages**

Create the homepage, about page, and six category pages with matching front matter.

- [ ] **Step 2: Create sample posts**

Create six Markdown posts, each with title, date, category, location, excerpt, hero image, and example inline image syntax.

- [ ] **Step 3: Verify categories**

Run: `rg "category: " _posts categories`
Expected: every requested category appears at least once.

- [ ] **Step 4: Commit**

Run: `git add index.md about.md categories _posts && git commit -m "feat: add travel pages and sample stories"`

### Task 4: Local Verification

**Files:**
- Modify only if verification finds an issue.

- [ ] **Step 1: Check file references**

Run: `rg "/assets/images/" .`
Expected: image references use `/assets/images/...` paths.

- [ ] **Step 2: Check git status**

Run: `git status --short`
Expected: clean working tree after commits, unless verification fixes were needed.
