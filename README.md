# GH Container extension

GH plugin to manange container packages

## Install
```bash
gh extension install nicovince/gh-container
```

## Usage
Display list of container packages for the authenticated user
```
gh container list
```

Display versions of a container package
```
gh container versions my-package-name
```

Clean untagged versions of a container package
```
gh container clean my-package-name --untagged
```

> Your Github Token must have the `delete:package` permission in order to perform the `clean` action.  
> The clean action fails from a github action, you may with to use [actions/delete-package-versions](https://github.com/actions/delete-package-versions)
