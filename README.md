# Ayah Fi Daqiqa — Public Worker

This repository contains only the GitHub Actions worker for the Ayah Fi Daqiqa video generator.

## Activation

1. Add repository Actions secret `AYAH_API_KEY` (do not commit the key).
2. Manually run **Ayah Scheduled Worker** once from Actions and verify it works.
3. Only after a successful test, enable the schedule. Keep the old private workflow disabled when switching, to prevent two workers claiming tasks.

The workflow is initially manual-only to avoid running before credentials are configured. Video output artifacts are not published from this public repository.
