
`  Execute this command {$env:NODE_OPTIONS="--openssl-legacy-provider"} before executing npm start`

After running this, any subsequent Node.js commands (e.g., npm install, node app.js) will use this option.
Alternatively, you can also set this environment variable directly in your project's package.json under the scripts section, for example:

"scripts": {
  "start": "set NODE_OPTIONS=--openssl-legacy-provider && node app.js"
}

This would automatically set the environment variable when running npm start.
