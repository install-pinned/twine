
# install-pinned/twine
<!-- !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! -->
<!-- ⚠️auto-generated from init.py, do not edit manually ⚠️-->
<!-- !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! -->

![](https://shields.io/badge/python-%3E=3.8-blue)
![](https://shields.io/badge/runner%20os-Windows%20%7C%20Linux%20%7C%20macOS-blue)

Securely install the latest [twine](https://pypi.org/project/twine/) release from PyPI.

This action installs a pinned version of **twine** and all its dependencies,         making sure that file hashes match. Pinning your dependencies:

 1. Stops software supply chain attacks.
 2. Makes sure your CI does not break unexpectedly.

## Usage

In your GitHub Actions workflow, use this action like so:

```yaml
      - name: Install twine from PyPI
        uses: install-pinned/twine@eea2eb0abb443a6a862fd596581e049e7a8e2bfa  # 6.1.0
```

You can [set up Dependabot](https://docs.github.com/en/code-security/dependabot/working-with-dependabot/keeping-your-actions-up-to-date-with-dependabot#example-dependabotyml-file-for-github-actions)
so that your pins are updated regularly.

## Alternatives

This action is a relatively simple wrapper around [uv](https://docs.astral.sh/uv/)         and is most useful if there is no existing `requirements.txt`/`uv.lock`/... infrastructure in place.         If you already pin all your dependencies in a single place, you don't need it!

## More Details

See the [@install-pinned README](https://github.com/install-pinned) for details.
