# vscode-stylelint-yarn-esm-bug

This repo demonstrates [stylelint/vscode-stylelint#464](https://github.com/stylelint/vscode-stylelint/issues/464)
where a Stylelint will fail to start a server in project that uses Plug'n'Play
ESM loaders.

This project is configured with the `stylelint-pretteier` plugin which
imports `prettier` using `import()` rather than `require()`.