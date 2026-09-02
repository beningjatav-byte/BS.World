# BS.World — fixed foundation

This version improves the original starter with:
- Supabase login/signup + password reset flow
- Profile editing
- Connection request duplicate protection
- Realtime connection-request refresh
- Connection-gated private messaging
- Realtime message subscription
- Message deduplication
- Basic browser camera/microphone call screen

## Supabase
Run `supabase_schema.sql` in the SQL Editor, then add:
VITE_SUPABASE_URL
VITE_SUPABASE_ANON_KEY

## Important
True user-to-user WebRTC calling still needs a signaling layer (offer/answer/ICE exchange) and production TURN configuration. The current call screen tests local camera/microphone access but does not pretend to be a completed remote call.
