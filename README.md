# My Docker Builder

## Specification
-----
### base-ubuntu (Ubuntu 20.04 (LTS) Focal Fossa)
#### Installed Package

* wget, bzip2, ca-certificates, locales, font-liberation, vim, git, zsh, oh-my-zsh
* net-tools, openssh-server openssh-client
#### Command
``` bash
docker run -it --rm --name base ajkimdev/base-ubuntu zsh
```