# Project Template
Here's a simple template with a Makefile. This allows you to create:

1. A self contained environment in which you can run notebooks
2. Work on a package inside the `\scripts` folder, where you can save functions/classes you want to use inside the jupyter notebook (this keeps your notebook relatively clean and free of a cascade of initial function defintions)

## Usage

```bash
make install  #installs everything and creates the environment
./jupyter lab # launches jupyter lab, you could do ./jupyter notebook too
```

Then in the jupyter notebook you can do whatever you want.
