# 途中雜誌

A GitHub Pages-ready Jekyll travel blog for photo-rich travel essays.

## Write A New Story

1. Copy one file from `_posts/`.
2. Rename it with this format: `YYYY-MM-DD-story-name.md`.
3. Edit the front matter:

```yaml
---
layout: post
title: "文章標題"
date: 2026-06-28
category: japan
category_name: 日本
location: 京都
excerpt: "首頁會看到的短摘要。"
hero_image: /assets/images/japan/your-photo.jpg
---
```

4. Put photos in `assets/images/`.
5. Insert a photo in the article:

```markdown
![照片說明](/assets/images/japan/your-photo.jpg)
```

## Categories

- 烏茲別克: `uzbekistan`
- 匈牙利: `hungary`
- 蔚藍海岸: `cote-d-azur`
- 日本: `japan`
- 美食: `food`
- 住宿: `stays`

## Publish On GitHub Pages

1. Create a GitHub repository named `your-username.github.io`.
2. Push this folder to that repository.
3. In GitHub, open `Settings` -> `Pages`.
4. Set source to `Deploy from a branch`, branch `main`.
5. Visit `https://your-username.github.io` after GitHub finishes building.
