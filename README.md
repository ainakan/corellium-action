# Corellium Action

This uploads and executes code on a Corellium instance.

# Usage

```yaml
steps:
- uses: ainakan/corellium-action@v4
- with:
    token: ${{ secrets.GITHUB_TOKEN }}
    gateway: corellium.ainakan.re
    device: android-arm64
    upload: runner.tar.gz
    run: |
      cd /data/android/ainakan
      tar xf $ASSET_PATH
      ./gum-tests
```
