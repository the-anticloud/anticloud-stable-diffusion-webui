# Developer Cookbooks — STABLE_DIFFUSION_WEBUI

**Project:** `STABLE_DIFFUSION_WEBUI`
**Category:** ARTIST_TOOLS
**Domain:** artist tools and creative software
**Date:** 2026-10-08

---

## Common Tasks

### Adding a New Feature
1. Create a feature branch
2. Write tests first (TDD)
3. Implement the feature
4. Run verification checks
5. Submit a pull request

### Debugging
```bash
python -m pdb src/stable_diffusion_webui/main.py
```

### Security Scanning
```bash
python tools/run_bench.py --only owasp
```

## Code Patterns

### Error Handling
All errors are logged to the AIOSS chain with full context.

### Configuration
Configuration is loaded from environment variables with sensible defaults.

### Testing
Tests use pytest with coverage reporting. Target: >80% coverage.

## Verification

16/16 PASS. Evidence: `ISOLATED_LAB_RESULTS/03_Result_Register.md`.
