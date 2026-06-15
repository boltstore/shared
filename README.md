# @boltstore/utils

Shared types, schemas, and utilities for the Boltstore ecosystem.

## What's inside

- **TypeScript types:** `Record`, `Pagination`, `Filter`, `Query`, auth types, realtime types, sync types, storage types
- **Filter parser:** Parse, compile, and convert Boltstore filter strings to SQL
- **Validation:** Collection name, field name, and filter validation utilities
- **Constants:** HTTP routes, WebSocket events, filter operators, and more
- **JSON Schema:** Cross-language type definitions for generating PHP, Go, and other SDKs

## Installation

```bash
npm install @boltstore/utils
```

## Usage

```typescript
import { parseFilter, compileFilter } from "@boltstore/utils";
import type { Filter } from "@boltstore/utils";

const filter = parseFilter("age:gte:18 AND status:eq:active");
console.log(compileFilter(filter));
// "(age:gte:18 AND status:eq:"active")"
```

## Development

```bash
bun install
bun run build    # compile TypeScript
bun test         # run tests
```

## Publishing

```bash
npm publish
```

## License

MIT