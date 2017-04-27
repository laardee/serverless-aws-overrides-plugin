Serverless AWS Overrides Plugin
=============================

This plugin fixes these known Serverless AWS issues:
- Serverless (node.js) runtime version is not updated when updating s-function.js

This plugin will contain the runtime fixes that are needed. Most of this is forked Serverless 0.5x code
that permits plugin overrides.

**Note:** Requires Serverless *v0.5.0*.

### Setup

Add the plugin into your package.json

```
  "serverless-plugin-aws-overrides": "git+ssh://git@github.com/blackevil245/serverless-plugin-aws-overrides.git",
```

Add the plugin to the `plugins` array in your Serverless Project's `s-project.json`, like this:

```
  plugins: [
      "serverless-plugin-aws-overrides"
  ]
```

Change a s-function.json configuration to verify the behaviour:

```
  "runtime": "nodejs4.3",
```
