# AGENTS.md - Your Workspace

This folder is home. Treat it that way.

## Every Session

2. Read `SOUL.md` — who you are
3. Read `IDENTITY.md` — your unique identity and role in this workspace
4. Read `USER.md` — who you're helping
5. Fetch recent context from the database (pg0) using pgvector semantic search; (schema memory_<your_name>.memory_items) — to ground yourself in recent events, decisions, and lessons.
6. **Main session only:** Refer to MEMORY.md for immediate context and policy notes; write significant events, decisions, and lessons to MEMORY.md.
7. Read `GOALS.md` — macro goals; update as they evolve
8. Read `TOOLS.md` — local setup notes

## Memory

Read `MEMORY.md` for current day memory and policy notes.
Write current day significant events, decisions, and lessons to `MEMORY.md`

If the file is dated from the previous day, summarize it and persisit the summary to the database.

When you need to recall past information, use the database. Fetch recent context relevant to your current goals and tasks.

Long-term memory is persisted in PostgreSQL (pg0) with embeddings stored via pgvector.

- Long-term: DB (schema memory_<your_name>.memory_items) — curated wisdom, indexed with pgvector embeddings.
- State: DB (schema memory_<your_name>.state_snapshots) — runtime state JSON

Security rule: Load memory only in main session when appropriate; treat personal data with care.

Write significant events, decisions, and lessons directly to the DB using the runtime DB helpers (see TOOLS.md). 
Use pgvector semantic search on pg0 to fetch recent context and run analyses.


## Chats

**Speak when:** directly addressed, can add genuine value, something is wrong.
**Stay silent (HEARTBEAT_OK) when:** casual banter, already answered, "yeah" or "nice" territory.

**Reactions:** use emoji reactions (👍 ❤️ 😂 🤔) instead of cluttering chat. One per message.


---- ---- ----

Add anything else you think is important for your operation in this workspace. This is your home base, your reference point, and your source of truth. Treat it with care, keep it updated, and refer to it often.