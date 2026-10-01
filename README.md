# Jesus and Mary College Voicebox

Anonymous complaint & suggestion box for the **Jesus and Mary College
Students' Union**. Static frontend in `public/`, three serverless API
routes in `api/`, shared auth helper in `lib/`, and data stored in
Upstash Redis.

Tracking codes are of the form `JMC-XXXXXX`. All Redis keys live under the
namespace `du:jmc:voicebox` so the app can safely share one Upstash
instance with other DU college deployments.

## Deploy in 5 minutes

### 1. Push to GitHub
```bash
git init
git add .
git commit -m "JMC Voicebox"
git branch -M main
git remote add origin https://github.com/anubhavbajpaibusiness/jesus-mary-opress.git
git push -u origin main