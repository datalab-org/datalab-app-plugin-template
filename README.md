# datalab-app-plugin-template

> [!WARNING]
> This repository is still under active development and will have some rough edges. 
Please raise any issues in the [Issue Tracker](https://github.com/datalab-org/datalab-app-plugin-template/issues?q=sort%3Aupdated-desc+is%3Aissue+is%3Aopen) or contact us via the routes listed at [datalab-org](https://github.com/datalab-org).

This template uses [Copier](https://github.com/copier-org/copier).

We recommend using `uv` to manage Python versions and environments, in which case the template can be used with:

```shell
mkdir my_plugin
uvx copier copy "git@github.com:datalab-org/datalab-app-plugin-template" <my_plugin>
```

This will guide you through the process of creating a new repository for your plugin.
You can commit the result, alongside the `.copier-answers.yml` file, to your new repository (after creating it on GitHub or elsewhere):

```shell
cd <my_plugin>
uv lock
git init
git add .
git commit -m "Initial commit"
git remote add origin <your-repo-url>
```

You can also occasionally sync changes from this template by running the following command in your plugin repository:

```shell
uvx copier update
```

Releases of the plugin are created via semantic version tags on GitHub, and will require manually updating the `CHANGELOG.md` file.

An example use of this repository can be found at [datalab-app-plugin-example](https://github.com/datalab-org/datalab-app-plugin-example).
