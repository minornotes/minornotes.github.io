# Travel Blog Design

## Goal

Build a GitHub Pages-ready travel writing website for publishing photo-rich travel essays in a magazine-like style.

## Chosen Approach

Use Jekyll, because GitHub Pages supports it directly and it keeps writing simple: each travel story is a Markdown file with front matter for title, date, category, location, excerpt, and hero image.

## Site Structure

- Home page: magazine-style hero section, featured stories, recent stories, and category entry points.
- Story pages: article title, date, location, hero photo, body copy, and inline photos.
- Category pages: one page per category showing matching stories.
- About page: short profile and writing focus.
- Photo folder: `assets/images/`, with placeholders and clear examples for where real travel photos should go.

## Categories

- 烏茲別克
- 匈牙利
- 蔚藍海岸
- 日本
- 美食
- 住宿

## First Version Content

Create one sample story per category so the user can copy, rename, and edit the files:

- 烏茲別克: 撒馬爾罕藍色清晨
- 匈牙利: 布達佩斯河邊散步
- 蔚藍海岸: 尼斯午後海岸線
- 日本: 京都秋日小路
- 美食: 旅途中記住的一餐
- 住宿: 一間醒來會想寫字的房間

## Visual Direction

The site should feel like a compact travel magazine: calm, editorial, photo-forward, and easy to scan. It should avoid a marketing landing-page feel. The first screen should show the blog identity, a large featured story, and a visible hint of the story grid below.

## Implementation Notes

Use a conservative Jekyll layout with no external dependencies. CSS should live in `assets/css/style.css`. The site should work locally as static files where possible, and on GitHub Pages when pushed to a repository.

## Success Criteria

- The project exists at `/Users/apple2/travel-blog`.
- It contains a valid Jekyll/GitHub Pages structure.
- It has the requested six categories.
- It includes sample articles showing how to add photos.
- It includes short instructions for publishing to GitHub Pages.
