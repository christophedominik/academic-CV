# Migration Package — Wowchemy v5 → HugoBlox Academic CV
# Generated with verified diffs against official HugoBlox docs

## What changed and why

| Item | Old | New |
|---|---|---|
| Publications folder | content/publication/ | content/publications/ |
| Blog posts folder | content/post/ | content/blog/ |
| Events folder | content/event/ | content/event/ (same) |
| Author profile location | content/authors/admin/_index.md | data/authors/admin.yaml |
| Author avatar | content/authors/admin/avatar.png | assets/media/authors/admin.png |
| Publication types | ["2"] numeric | ["article-journal"] named |
| Icon format | icon_pack: fab + icon: twitter | icon: brands/x |
| Education | education.courses: | education: flat list |
| Empty links | links: | links: [] |
| Old shortcodes | {{< staticref >}} etc | removed |

## STEP 1 — DELETE from your new template repo:
- content/blog/          (broken example files — causes cite shortcode crash)
- content/courses/       (broken example files)
- content/slides/        (broken example files)
- content/admin/         (old CMS file — causes wowchemycms_config error)

## STEP 2 — COPY from this zip into your repo root:
Drag the following into your repo folder, merging when asked:
- content/publications/  (was content/publication/)
- content/event/         (same name, fixed syntax)
- content/blog/          (was content/post/)
- content/project/       (same name, fixed syntax)
- content/authors/admin/ (updated profile format)
- data/authors/          (NEW location for author profiles)
- assets/media/authors/  (NEW location for author avatars)

## STEP 3 — Commit and push
In GitHub Desktop: commit all → push
