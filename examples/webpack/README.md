## Webpack version
This command will show the current available version of Webpack.

```bash
npm view webpack version
```
### 1. Create a new project
Create a new directory for the project and initialize NPM:

```bash
mkdir my-project
cd my-project
npm init -y
```

### 2. Install the necessary dependencies
Install Webpack and related packages:

```bash
npm install --save-dev webpack webpack-cli
```

### 3. Protect your project from unintentional publication
In the ***package.json***, the "private": true parameter is set to true. This parameter indicates that this package is private and is not intended to be published in a public repository, such as the npm registry. When this parameter is set to true, the npm publish command is rejected, preventing accidental publishing of the package.

This option is useful when you are developing an internal project or library that should not be publicly available. For example, if you are creating a project for your company's internal use, you may need to set "private": true to avoid accidentally publishing it to the public npm registry.

Thus, this line protects your project from unintentional publication.

```json
{
    ...
  "private": true,
    ...
}
```