# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some Oxlint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Oxc](https://oxc.rs)
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/)

## React Compiler

The React Compiler is not enabled on this template because of its impact on dev & build performances. To add it, see [this documentation](https://react.dev/learn/react-compiler/installation).

## Expanding the Oxlint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and Oxlint's TypeScript related rules in your project.

## Environment Variables Configuration

Copy `.env.example` to `.env.local` and fill in your actual credentials:

```bash
cp .env.example .env.local
```

Required Variables:
- `VITE_SUPABASE_URL`: Your Supabase Project URL
- `VITE_SUPABASE_ANON_KEY`: Your Supabase Public Anonymous Key

> **IMPORTANT**: Ensure Row Level Security (RLS) is enabled on all tables in Supabase prior to production deployment.

## ⚠️ Security Notice: Git History & Secret Rotation

> **WARNING**: If any API keys, tokens, or credentials were previously hardcoded or committed to git history at any point, those historical values **remain exposed in the git commit log**. You MUST immediately **rotate all previously hardcoded secrets** (e.g. regenerate Supabase API keys, database credentials, OAuth client secrets, or API tokens) before deploying this application to production.

