# Trek Course Guides

Community-written study guides for FAST-NUCES Karachi courses, surfaced inside
[Trek](https://github.com/Trek-Developers) on the course resources page.

This repo holds the content. Trek's backend reads it read-only — there's no
in-app editor and no moderation queue on Trek's side. Every change here goes
through a normal GitHub pull request.

## How this works

- One guide per course, at `guides/{COURSE_CODE}/guide.md`.
- Trek links directly into GitHub's own "create/edit file" flow — you don't
  need to clone this repo or use git locally. Click **"Write the first
  guide"** or **"Suggest an Edit"** on a course page in Trek, and GitHub
  will auto-fork this repo and open a pull request draft for you.
- A guide doesn't need to be complete to submit. A first draft with just the
  Overview filled in is a legitimate PR.

## Structure

```
trek-course-guides/
├── README.md                        this file (index below is auto-generated)
├── TEMPLATE.md                       starter template for new guides
├── .github/
│   ├── PULL_REQUEST_TEMPLATE.md
│   └── workflows/update-readme.yml   regenerates the index below on merge
└── guides/
    ├── CS101/guide.md
    ├── CS205/guide.md
    └── ...
```

## Writing or editing a guide

1. Use [`TEMPLATE.md`](./TEMPLATE.md) as your starting structure — Trek
   pre-fills it automatically when you click "Write the first guide," so you
   likely won't need to open this file directly.
2. Keep the four sections (`Overview`, `Topics & Resources`, `Tips`,
   `Useful Links`) — this keeps guides consistent across courses.
3. **Don't change the `# {CODE} — {Name}` heading format** — it's parsed
   automatically to build the index below. Editing the course name is fine;
   changing the heading structure itself will break the index.
4. Link out to existing Trek resources (notes, past papers already uploaded)
   rather than re-uploading or re-pasting content — this repo is for
   guidance and context, not file hosting.

## Guides

<!-- AUTO-GENERATED:START -->
| Code | Course | Guide |
|------|--------|-------|
| AI2002 | Artificial Intelligence | [View](guides/AI2002/guide.md) |
<!-- AUTO-GENERATED:END -->

## License

Guide content in `guides/` is contributed by students for students. See
[LICENSE](./LICENSE) for terms.
