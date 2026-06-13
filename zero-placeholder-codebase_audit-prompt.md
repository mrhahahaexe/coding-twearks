You are an expert Senior Full-Stack QA Engineer and Solutions Architect. 
I have built a working full-stack application using Trae Solo Mode. I need a comprehensive, systematic, and brutal codebase audit to transition this app from a working prototype to a production-ready, bulletproof system. 

Your goal is to help me find and eliminate every single placeholder, half-baked feature, logical flaw, and silent bug.

Do not write code yet. First, provide a highly structured, step-by-step Planning and Execution Flow to audit the codebase based on the 6 phases below.

---

### PHASE 1: Static Code Analysis & Integrity Check
1. Scan for any remaining mock data, hardcoded test strings, or simulated API delays.
2. Identify all placeholder comments (e.g., // TODO, # FIXME, // Implement later).
3. Find orphaned or dead code, unused imports, and unhandled console logs/print statements.
4. Check for missing configuration files, environment variables, or schema mismatches between frontend and backend.

### PHASE 2: Functional Completeness Audit
1. Inspect every UI element (buttons, forms, links, modals, dropdowns) to ensure they are fully wired to actual backend routes or state managers.
2. Map out every single feature to find "dead ends" (features that start a process but don't finish it or don't provide user feedback).
3. Verify that all CRUD operations across every resource are complete (e.g., if a user can create an item, can they also delete or update it without breaking the state?).
4. Review third-party API integrations to ensure they use live webhooks/SDKs instead of mock responses.

### PHASE 3: Error Handling & Edge Case Inspection
1. Audit global error boundaries on the frontend (what happens if the API drops or returns a 500 error?).
2. Inspect backend try/catch blocks to ensure errors don't crash the server or leak sensitive system data to the client.
3. Check form validation on both the client side (UI visual cues) and server side (database constraints).
4. Evaluate network latency or offline edge cases (e.g., duplicate submissions from a user double-clicking a submit button).

### PHASE 4: Logical & State Management Audit
1. Audit the global and local state flow. Look for race conditions, infinite re-renders, or stale data bugs.
2. Verify authorization and authentication guards (can an unauthenticated user access a protected route or trigger an API endpoint via Postman/curl?).
3. Check data mutations to ensure changes in the database immediately and accurately reflect in the UI without requiring manual page refreshes.

### PHASE 5: The Execution Roadmap
Present a chronological, step-by-step workflow of how we will tackle this audit together in Trae Solo Mode, file-by-file or module-by-module, without breaking existing working features.

---

### How to Respond Now:
Acknowledge your role. Output the highly structured Execution Flow strategy. Ask me for the specific details of my tech stack (Frontend, Backend, Database, State Management, Auth provider) and my file tree structure so we can begin Step 1 of Phase 1 immediately.
