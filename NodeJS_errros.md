# Error: error:0308010C:digital envelope routines::unsupported
- You can try one of these:

 1. Enable legacy OpenSSL provider.

- On Unix-like (Linux, macOS, Git bash, etc.):

- export NODE_OPTIONS=--openssl-legacy-provider
- On Windows command prompt:

- set NODE_OPTIONS=--openssl-legacy-provider
- On PowerShell:

- $env:NODE_OPTIONS = "--openssl-legacy-provider"

- In your package.json: change this line

- "start": "react-scripts start"
- to

- "start": "react-scripts --openssl-legacy-provider start"

-  2. Downgrade to Node.js v16.

- You can reinstall the current LTS version from Node.js’ website.

- You can also use nvm. For Windows, use nvm-windows.
