```sh-session
$ yarn
$ yarn playwright test
yarn run v1.22.19
Error: Cannot find module 'app/my-pkg'
Require stack:
- /Users/oliver/Code/Reduced test cases/playwright-pkg-require-with-path/tests/example.spec.ts
- /Users/oliver/Code/Reduced test cases/playwright-pkg-require-with-path/node_modules/@playwright/test/lib/transform/transform.js
- /Users/oliver/Code/Reduced test cases/playwright-pkg-require-with-path/node_modules/@playwright/test/lib/common/config.js
- /Users/oliver/Code/Reduced test cases/playwright-pkg-require-with-path/node_modules/@playwright/test/lib/reporters/json.js
- /Users/oliver/Code/Reduced test cases/playwright-pkg-require-with-path/node_modules/@playwright/test/lib/reporters/raw.js
- /Users/oliver/Code/Reduced test cases/playwright-pkg-require-with-path/node_modules/@playwright/test/lib/reporters/html.js
- /Users/oliver/Code/Reduced test cases/playwright-pkg-require-with-path/node_modules/@playwright/test/lib/runner/reporters.js
- /Users/oliver/Code/Reduced test cases/playwright-pkg-require-with-path/node_modules/@playwright/test/lib/runner/runner.js
- /Users/oliver/Code/Reduced test cases/playwright-pkg-require-with-path/node_modules/@playwright/test/lib/cli.js
- /Users/oliver/Code/Reduced test cases/playwright-pkg-require-with-path/node_modules/@playwright/test/cli.js

   at example.spec.ts:2

  1 | // ❌ Using path, it doesn't work.
> 2 | import * as x from 'app/my-pkg';
    | ^
  3 | // ✅ Not using path, it works.
  4 | // import * as x from '../app/my-pkg';
  5 |

    at Object.<anonymous> (/Users/oliver/Code/Reduced test cases/playwright-pkg-require-with-path/tests/example.spec.ts:2:1)

Error: No tests found







To open last HTML report run:

  npx playwright show-report

error Command failed with exit code 1.
```
