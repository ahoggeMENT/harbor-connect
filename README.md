# Harbor connector sign-in

The page Supabase sends a person to when they connect Harbor in ChatGPT or
Claude: sign in with Google, then approve or deny the connection.

It is generated, not edited here. The source is Harbor's
`supabase/functions/office-mcp/connect/` and it is exported with:

    node scripts/office-mcp/export-page.mjs --out <this folder>

It holds only public values (the Supabase project URL and its publishable
key). Every permission is decided by Supabase Auth and the database's
row-level security, not by this page.
