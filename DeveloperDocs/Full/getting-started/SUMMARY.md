# Table of contents

* [Concepts](README.md)
* [Guides](guides/README.md)
  * [Create a custom unfurl action for your integration](guides/create-a-custom-unfurl-action-for-your-integration.md)
  * [Use GitHub Actions to translate GitBook pages](guides/use-github-actions-to-translate-gitbook-pages.md)
* ```yaml
  type: builtin:openapi
  props:
    models: true
  dependencies:
    spec:
      ref:
        kind: openapi
        spec: priot
  ```
