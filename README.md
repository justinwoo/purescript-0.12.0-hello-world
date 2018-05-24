# PureScript 0.12.0 Hello World

You can get started with PureScript 0.12.0 easily by using this repo.

If you have everything installed, you should be able to follow this:

```
> psc-package install
Installing 3 packages...
...
Install complete
> pulp run
* Building project in /home/justin/Code/purescript-0.12.0-hello-world
...
* Build successful.
look, show on Record:
{ apple: "banana" }
```

## FAQs

### Do I need Bower?

No, unless you know exactly what you might use Bower for, you do not need it at all. You should be using Psc-Package like this repo does.

## "Installation"

Install `purescript`, `pulp`, and `psc-package` to get started.

One way you might install things you need is to use `npm` to install `pulp` (and `psc-package` if you wish)

`npm i -g pulp [psc-package]`

And for installing `PureScript`, you can have the cleanest setup by simply downloading the correct binary archive:

```
env:
  - PATH=$HOME/purescript:$HOME/psc-package:$PATH

install:
  - TAG=v0.12.0
  - PSC_PACKAGE_TAG=v0.3.2
  - wget -O $HOME/purescript.tar.gz https://github.com/purescript/purescript/releases/download/$TAG/linux64.tar.gz
  - tar -xvf $HOME/purescript.tar.gz -C $HOME/
  - chmod a+x $HOME/purescript
  - wget -O $HOME/psc-package.tar.gz https://github.com/purescript/psc-package/releases/download/$PSC_PACKAGE_TAG/linux64.tar.gz
  - tar -xvf $HOME/psc-package.tar.gz -C $HOME/
  - chmod a+x $HOME/psc-package
```

