# DeskLife Remote Config

Remote configuration hosting for the DeskLife application suite.

## Live Configuration URLs

### Production Configuration
```
https://imeralabs.github.io/desklife-remote-config/config/config.prod.json
```

### Schema Definition
```
https://imeralabs.github.io/desklife-remote-config/schema/config.schema.json
```

## Repository Structure

- `/config/` - Configuration files by environment
- `/schema/` - JSON schema definitions
- `/.github/` - GitHub Actions for validation and deployment

## Usage

The DeskLife apps fetch configuration from the GitHub Pages URLs above with:
- ETag caching support (10-minute cache expiry)
- HTTPS-only access
- Fallback to bundled configuration on network failure

## Configuration Features

- **Protocols**: Sitting/standing/moving timing definitions (20-8-2 default)
- **Feature Flags**: Toggle functionality across app versions
- **Guardrails**: Safety limits for prolonged sitting/standing
- **Score Bands**: Thresholds for performance scoring
- **Scheduling**: Prompt timing and quiet hours configuration

---
Last Updated: 2025-08-27