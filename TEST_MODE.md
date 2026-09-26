# TEST MODE

Set `TEST_MODE=1` in Railway Variables and redeploy.

In TEST MODE:
- MEXC is NOT queried.
- No exchange order can be placed.
- One deterministic test LONG message is sent to Telegram.
- The message is clearly marked `TEST MODE`.
- The process exits after sending the test message.

After confirming the Telegram message arrived, remove `TEST_MODE` (or set it to `0`) and redeploy for normal alert-only scanning.
