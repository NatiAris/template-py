# template-py

This repo is an example of a project that uses a Jupyter notebook as sandbox.  
Write code as a package, import it from the notebook, experiment, update the package, reload the package, GOTO 30.  
You'll probably want to see your sandboxes in gitignore, so just take the notebook, remember the structure and go read about [reloading-related caveats].

Alternative solution would be to use IPython's `%autoreload` magic.  
But it reloads modules at cell execution if changes were detected which is implicit and *Explicit is better than implicit*.  
You may chose to do something like `%notebook -e history.ipynb` if sandbox gets messy and I bet you would prefer to see explicit reloads instead of sudden behavoiur changes.  
The magic's documentation mentions [more reloading-related caveats].

Hope this helps.

[reloading-related caveats]: https://docs.python.org/3/library/importlib.html#importlib.reload
[more reloading-related caveats]: https://ipython.readthedocs.io/en/stable/config/extensions/autoreload.html#caveats
