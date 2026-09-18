# Push your code to GitHub and deploy your site

A four-part, step-by-step guide that takes a personal website from a folder on a
laptop to a live URL. Written for students with no terminal experience.

Created by Christopher Kang — MIT Sloan 2027, for 15.S23 AI Builder Space.

## The four parts

| Part | Steps | Where |
|------|-------|-------|
| 1. Create the repository | 1–3 | On GitHub |
| 2. Connect Claude Code | 4 | In Claude Code |
| 3. Push your code | 5–6 | In Claude Code |
| 4. Deploy to Vercel | 7–13 | On Vercel |

## How it works

One page per part. Each page shows a single step at a time, and will not advance
until every confirmation box on that step is ticked — so a step cannot be skipped
by scrolling, and a part cannot be opened until the parts before it are finished
(typing a part's URL directly shows a locked panel instead).

Progress is kept in the reader's own browser via `localStorage`, under the key
`push-deploy-v3`. Nothing is sent anywhere and there is no account or server state.

## Files

```
index.html     cover, the four part cards, and the "before you begin" checks
part-1.html    steps 1-3
part-2.html    step 4
part-3.html    steps 5-6
part-4.html    steps 7-13
done.html      the completion page
img/           screenshots of the Vercel screens
```

Plain static HTML — no build step, no dependencies, no environment variables.
CSS and JavaScript are inlined in each page on purpose: a stylesheet that failed
to load would make every step visible at once and defeat the gating.

## Running it locally

```
python3 -m http.server 8000
```

Then open <http://localhost:8000>. Opening `index.html` as a `file://` URL also
works, but page-to-page navigation and `localStorage` behave more like the real
thing over HTTP.

## Deploying

It is a static site, so any host works. Import this repository into Vercel and
accept every default — there is nothing to configure.
