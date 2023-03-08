# Flux Python Bindings

Hello! You've found the flux Python bindings, an experiment to build and deploy
Flux to Pypi without needing to store code alongside Flux. The goal of
this experiment is to test them separately.

## Development

We provide a [.devcontainer](.devcontainer) environment you can open in VSCode
to have an environment ready to go with Flux (and Flux Security). You can follow
the instructions in the DevContainer to build the Flux Python bindings.

### Building Modules


You can build:

```bash
$ python3 setup.py build
```

And then start a flux instance:

```bash
$ flux start --test-size=4
```

And then cd into the build directory:

```bash
$ cd build/lib.linux-x86_64-3.8/
```

And import flux.

```bash
$ ipython
```
```python
import flux
flux.Flux()
```

More coming soon! We still need to:

 - [ ] customize install to take paths to your install
 - [ ] some version checking
 - [ ] a complete build -> install workflow


