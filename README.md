# Community-Contributed Kestrel Huntbooks

This repository hosts community-contributed [Kestrel](https://github.com/opencybersecurityalliance/kestrel-lang) huntflows/huntbooks/patterns. For Kestrel analytics, visit the sister repo [kestrel-analytics](https://github.com/opencybersecurityalliance/kestrel-analytics/).

- [What is Kestrel?](https://kestrel.readthedocs.io/en/latest/overview.html)
- [What is a hunt/huntstep/huntflow/huntbook?](https://kestrel.readthedocs.io/en/latest/language.html#hunt)
- [The introduction talk at RSA 2021](https://www.rsaconference.com/Library/presentation/USA/2021/The%20Game%20of%20Cyber%20Threat%20Hunting%20The%20Return%20of%20the%20Fun)
- [The RSA demo (15 min)](https://www.youtube.com/watch?v=tASFWZfD7l8)
- [Kestrel technical blogs at OCA](https://opencybersecurityalliance.org/posts/)

### Binder (Under Testing)

https://mybinder.org/v2/gh/opencybersecurityalliance/kestrel-huntbook/HEAD?filepath=huntbooks

### How to Display Kestrel Huntbook With Syntax Highlighting

```shell
$ pip install -U pip setuptools wheel
$ pip install kestrel-jupyter
$ python -m kestrel_jupyter_kernel.setup
```
Then clone this repo and run `jupyter notebook` to open any huntbook. Note that _JupyterLab_ (Jupyter’s next-generation notebook interface) is not fully supported yet.

More setup information can be found at
- [Kestrel installation documentation](https://kestrel.readthedocs.io/en/latest/installation.html)
- [Kestrel hunting tutorial](https://kestrel.readthedocs.io/en/latest/tutorial.html#kestrel-jupyter)
- [Kestrel hunting stack setup](https://opencybersecurityalliance.org/posts/kestrel-2021-07-26/)
