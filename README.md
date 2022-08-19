# Project Template
Here's a simple template with a Makefile. This gives you:

1. A self contained environment in which you can run notebooks
2. Allows you to work on a package inside the `\scripts` folder, where you can save functions/classes you want to use inside the jupyter notebook (this keeps your notebook relatively clean and free of a cascade of initial function defintions)

## Usage
#### Initial Install
First add whatever packages you will need inside the `requirements.txt`

Then:
```bash
make install  #installs everything and creates the environment
```
You only need to do this once (or whenever you add another package to `requirements.txt`)

#### Running the notebook
Once installed, you can simply run:

```bash
./jupyter lab # launches jupyter lab in that environment, you could do ./jupyter notebook too
```

Then in the jupyter notebook you can do whatever you want.

#### Saving useful functions and classes
Add any classes or functions to the `/scripts` folder as you would in a package. 
Then in the notebook you can do:
```python
from scripts import *
```
and all the functions and classes will be available to you inside the notebook. This keeps your notebook relatively clean and free of a cascade of initial function defintions. 

Simply restart the notebook kernel and any changes you have made to `/scripts` will be updated. 

