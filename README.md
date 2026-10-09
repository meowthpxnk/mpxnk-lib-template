# My own python library tempolate

## Usage

1. Add new repository in PyPI
   Go to https://pypi.org/manage/account/publishing
   Add new GitHub repository
    - Project name - Your project name
    - Owner - Your github username
    - Repository - Repository name
    - Workflow name - `publish.yaml`
    - Environment name - `publish`

2. Run renaming script

```sh
poetry run rename_lib
```

3. Replace `LIB_DESCRIPTION` in pyproject.toml with your library description.

4. Update and push your project.

5. Go to github repository actions and run CI/CD workflow.

## Workflow usage

Workflow has
