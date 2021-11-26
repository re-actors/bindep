# `bindep`

A GitHub Action that lets you pre-provision the current CI VM with
OS packages listed in `bindep.txt` using [bindep].


## Usage

To use the action add the following step to your workflow file (e.g.
`.github/workflows/ci-cd.yml`)


```yml
- name: Provision OS packages from `bindep.txt`
  uses: re-actors/bindep@release/v1
  with:
    file: bindep.txt
    profile: test
```


## Options

There are two options — `file` and `profile`. Both are optional. See
[bindep] for more details.


## Related community projects

Check out the [tox-bindep] to have [bindep]-based checks in your
[tox] setup.


## License

The Dockerfile and associated scripts and documentation in this project
are released under the [BSD 3-clause license].


[bindep]: https://pypi.org/p/bindep
[BSD 3-clause license]: LICENSE.md
[tox]: https://tox.wiki
[tox-bindep]: https://github.com/tox-dev/tox-bindep
