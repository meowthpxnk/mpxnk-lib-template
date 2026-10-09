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

3. ❗️ALERT❗️Replace `LIB_DESCRIPTION` in pyproject.toml with your library description.

4. ❗️ALERT❗️Replace README.md with your package docs.

5. Create commit with message such as `feat!: Init project`. Push.

6. Go to github repository actions and run CI/CD workflow.

## Workflow usage

Workflow has environment variables:

- run-lint - Run linting
- run-tests - Run pytests tests
- run-release - Create release version
- run-build - Build project into tmp folder
- publish-to-pypi - Finally publish to pypi

You can run some jobs if you need, only lint or only tests.

## For customise Changelog

1. Run workflow with variables

- ✅ Lint
- ✅ Tests
- ✅ Release
- ✅ Build
- ❌ Publish

2. Pull repository

```sh
git pull
```

3. Change changelog custom

4. Commit changes

5. Run workflow with variables

- ✅ Lint
- ✅ Tests
- ❌ Release
- ✅ Build
- ✅ Publish
