# Steps to reproduce the issue

1. Clone this repo.
2. Install depedencies.
3. Run the `build` npm script.

## Expected behavior

- tsc is able to compile source code.

## Current behavior

- tsc crashes with the following error: 

```
src/index.ts:1:23 - error TS1479: The current file is a CommonJS module whose imports will produce 'require' calls; however, the referenced file is an ECMAScript module and cannot be imported with 'require'. Consider writing a dynamic 'import("@faker-js/faker")' call instead.
  To convert this file to an ECMAScript module, change its file extension to '.mts', or add the field `"type": "module"` to '/home/bob/Documents/repos/faker-js-faker-3087-repro/package.json'.

1 import { faker } from "@faker-js/faker";
                        ~~~~~~~~~~~~~~~~~
```