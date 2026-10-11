# Zood-Pay-at-table-web

Flutter web build of **Zood Pay-At-Table**, served as a static site by Vercel.

This repo only holds the compiled output (`flutter build web --release`).
Do not edit files here; change the Flutter app and redeploy:

```bash
# from the zood_pay_at_table app repo
tool/deploy_web.sh "commit message"
```

`vercel.json` rewrites every route (e.g. `/pay-at-table/<qr_id>/menu`) to
`index.html` so QR links open directly, and serves `/.well-known/*` as JSON
for App Links / Universal Links.
