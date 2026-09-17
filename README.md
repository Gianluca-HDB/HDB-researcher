# HDB Researcher v6.9.3

GitHub Pages ready: upload `index.html` to the repository root.

Integration hardening:
- separate Supabase auth storage from Participant
- researcher-selected participant dataset uses sessionStorage as an isolated working copy
- prevents Participant/Researcher HDB local data from colliding on the shared github.io origin
- researcher remains read-only at the Supabase policy layer for participant records
- HDB scientific baseline algorithm unchanged
