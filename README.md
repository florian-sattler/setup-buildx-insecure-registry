# Setup Buildx with Insecure Registry

A simple GitHub action calling the setup buildx action and configuring an insecure registry.

> [!NOTE]  
> This action may be useful if you are using github actions in an isolated environment with an insecure registry. Do not use this action for public registries!

## Example

```yaml
- name: Setup Insecure Registry
  uses: florian-sattler/setup-buildx-insecure-registry@v1.0.0
  with:
    url: 192.168.1.2:5000
```

## Arguments

### `url` (_required_)

The URL of the insecure registry. E.g. `192.168.1.2:5000` or `my-registry.local:3000`.
