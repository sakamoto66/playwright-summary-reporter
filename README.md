# Playwright-Summary-Reporter

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE.md)

The Playwright-Summary-reporter is designed to generate and report summaries of Playwright test results.

```bash
All 20 ✅ 8 ❌ 6 ⚠ 2 ⏭  4 ⏱  0m 14s
```

## Usage

1. Install the playwright-summary-reporter library:

```shell
npm i -D @sakamoto66/playwright-summary-reporter
```

2. To use a reporter define it in playwright.config.ts as reporter:

- playwright.config.ts

```typescript
import { defineConfig, devices } from '@playwright/test';

export default defineConfig({
  reporter: [
    [ '@sakamoto66/playwright-summary-reporter' ]
  ],
})
```

## Options

| Option           | Required | Description                                                     |
|------------------|----------|-----------------------------------------------------------------|
| outputFile       | Optional | Outputs the summary of test results to a file. If omitted, it outputs to the standard output. |

## License

The playwright-summary-reporter project is under the MIT License. For more details, refer to the [LICENSE](LICENSE.md) file.

