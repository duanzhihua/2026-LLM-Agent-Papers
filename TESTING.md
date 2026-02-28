# OpenClaw Test Coverage

This repository contains comprehensive test coverage for the OpenClaw platform.

## 📊 Test Statistics

- **Total Test Files**: 78
- **Total Lines Added**: 17,401
- **Coverage**: All major modules and extensions

## 🧪 Test Categories

### 1. Core Tests (`test/`)
- **gateway.multi.e2e.test.ts** - Multi-provider gateway end-to-end tests
- **auto-reply.retry.test.ts** - Auto-reply retry mechanism tests
- **inbound-contract.providers.test.ts** - Inbound contract provider tests
- **provider-timeout.e2e.test.ts** - Provider timeout handling tests
- **media-understanding.auto.e2e.test.ts** - Media understanding auto tests
- **test-env.ts** - Test environment setup
- **global-setup.ts** - Global test setup
- **setup.ts** - Test setup file

### 2. Extension Tests (`extensions/*/`)
Comprehensive tests for all OpenClaw extensions:

- **BlueBubbles**: Actions, attachments, chat, monitor, reactions, send, targets
- **Diagnostics-OTEL**: Service tests
- **Google Chat**: API, monitor, targets
- **LINE**: Channel logout, sendPayload
- **LLM Task**: LLM task tool tests
- **Lobster**: Lobster tool tests
- **Matrix**: Channel directory, resolve-targets
- **Mattermost**: Channel tests
- **Memory-LancedB**: Database extension tests
- **MSTEAMS**: Attachments, channel directory, conversation store, errors, file consent, inbound, media helpers, messenger, policy, polls, probe, sent message cache
- **Nextcloud Talk**: Policy tests
- **Nostr**: Channel, bus (test, integration, fuzz), profile (HTTP, import, fuzz), state store, types
- **TLOn**: Config schema tests
- **Twitch**: Access control, config, onboarding, outbound, plugin, probe, send, status, token, twitch-client
- **Voice Call**: Config, manager, media stream, webhook security
- **Zalo**: Channel directory, monitor webhook
- **ZaloUser**: Channel, status issues

## 🚀 Running Tests

```bash
# Run all tests
npm test

# Run specific test file
npm test gateway.multi.e2e.test.ts

# Run with coverage
npm test -- --coverage
```

## 📝 Test Structure

Each test file follows the standard OpenClaw testing pattern:

1. **Setup**: Initialize test environment
2. **Test Cases**: Individual test scenarios
3. **Teardown**: Clean up test resources
4. **Helpers**: Utility functions for tests

## 🎯 Coverage Goals

- [x] Core module coverage
- [x] Extension coverage
- [x] E2E test coverage
- [x] Integration test coverage
- [x] Fuzz testing for critical paths

## 📖 Documentation

For detailed testing documentation, see:
- `README_TEST.md` - Testing guide
- `TESTING.md` - This file

---

**Last Updated**: 2026-02-28
**Maintained By**: OpenClaw Team
