# LLM Clients - Consistency Improvements

## Completed

### 1. `validate_model()` warning path
- `create_llm_client()` now calls `validate_model()` and emits a warning for
  unknown model names instead of failing immediately.

## Remaining Issues to Fix

### 2. ~~Inconsistent parameter handling~~ (Fixed)
- GoogleClient now accepts unified `api_key` and maps it to `google_api_key`

### 3. ~~`base_url` accepted but ignored~~ (Fixed)
- All clients now pass `base_url` to their respective LLM constructors

### 4. ~~Update validators.py with models from CLI~~ (Fixed)
- Synced in v0.2.2
