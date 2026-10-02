# LoFo on Vercel

This directory is the Vercel project root for the public LoFo deployment.

It uses a Vercel external rewrite so the application continues to use its
Cloudflare D1 and R2 bindings without changing the public Vercel URL.

When importing the repository into Vercel, set **Root Directory** to
`deploy/vercel` and leave the framework preset as **Other**.

The `public` directory satisfies Vercel's static output requirement; requests
are still handled by the external rewrite in `vercel.json`.
