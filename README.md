# Jesus and Mary College Voicebox

Anonymous complaint & suggestion box for Jesus and Mary College.
Static frontend in `public/`, serverless API in `api/`, helpers in `lib/`,
data in Upstash Redis (one database shared by all college sites).

| Setting | Value |
|---|---|
| Tracking-code prefix | `JMC-XXXXXX` |
| Redis namespace | `du:jmc:voicebox` |
| Repo / Vercel project | `jesus-mary-opress` |

## Deploy
1. Push this folder to GitHub (`https://github.com/anubhavbajpaibusiness/jesus-mary-opress.git`) and import it in Vercel.
2. Environment variables:
   - `UPSTASH_REDIS_REST_URL`, `UPSTASH_REDIS_REST_TOKEN` — identical on every college project
   - `ADMIN_PASSWORD` — unique per college (use a long one)
   - `REDIS_NAMESPACE` — optional override, defaults to `du:jmc:voicebox`. Never reuse another college's value.

## Office bearers
Edit the `TEAM` array in `public/index.html`. Put photos in `public/images/team/`
and set `photo: "/images/team/president.jpg"`. An empty `TEAM` shows a "coming soon" card.
