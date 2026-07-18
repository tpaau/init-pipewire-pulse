# init-pulse

Initialize a PulseAudio server in GitHub Actions.

May be useful for testing apps that need a working sound server with a sink on the system.

Example usage:
```yaml
name: Example

on: [push, pull_request]

jobs:
  test:
    name: Do some testing
    runs-on: ubuntu-latest
    steps:
    - uses: actions/checkout@v6
    - uses: tpaau/init-pulse@main

    - name: Do some testing
      run: echo "All tests passing!"
```
