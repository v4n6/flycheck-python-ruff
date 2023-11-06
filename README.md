# flycheck-python-ruff
Flycheck checker for python ruff linter that supports error explanations.

# Install
## MELPA
```
M-x package-install flycheck-python-ruff
```

## Manual
```
M-x package-install-file
```

# Usage
Add the following lines to your config
```lisp
(eval-after-load 'flycheck                                       
  '(add-hook 'flycheck-mode-hook #'flycheck-python-ruff-setup))
```

If you have `use-package` installed
```lisp
(use-package flycheck-python-ruff
  :ensure t
  :hook ((python-mode python-ts-mode) . flycheck-python-ruff-setup))
```

# Contribute
Pull requests are welcomed.
