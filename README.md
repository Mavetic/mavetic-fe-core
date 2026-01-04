@mavetic/mavetic-fe-core
=========================

FE core utilities
-----------------
Contains default Biome and TypeScript configurations.

Features
--------
- Biome configuration exported as "biome" alias
- TypeScript configuration exported as "tsconfig" alias

Usage
-----
Biome example:
```json
{
  "extends": ["@mavetic/mavetic-fe-core/biome"]
}
```

TypeScript example
```json
{
  "extends": "@mavetic/mavetic-fe-core/tsconfig",
  "compilerOptions": {
    "paths": {
      "@/*": ["./src/*"]
    }
  },
  "include": [
    "next-env.d.ts",
    "src/types/*.d.ts",
    "**/*.ts",
    "**/*.tsx",
    ".next/types/**/*.ts"
  ],
  "exclude": ["node_modules"]
}

```
Publishing
----------
Has no build, only files are published and aliased.

License
-------
This project is licensed under MIT license (see LICENSE file)
