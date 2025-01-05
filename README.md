## Next.js 15 App Directory: Custom Server Issue

This repository demonstrates an unexpected behavior when using a custom server with the Next.js 15 app directory and `next dev`.  The application renders correctly in production, but the development server behaves erratically.

**Problem:**
When running `next dev`, the custom server is not correctly handling requests, potentially resulting in error 500s or incorrect responses.  This issue is specific to the app directory.

**Reproduction Steps:**
1. Clone this repository.
2. Run `npm install`.
3. Run `next dev`.
4. Observe unexpected behavior in the browser (errors, incorrect rendering). 

**Expected behavior:**
The custom server should correctly handle requests during development, providing a similar experience to production. 

**Possible causes:**
- Misconfiguration of the custom server.
- Incompatibilities between the custom server and the app directory.
- Issues related to the `next dev` process.