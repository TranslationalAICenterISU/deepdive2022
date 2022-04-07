
# CyVerse Container Camp 2022

MKDocs website for Container Camp 2022 - both basic and advanced materials here 

TBD: pretty much everything, set up action, set GH Pages to DNS, build website, add pages, convert all `rst` materials and update

htps://cyverse.org/cc

# Development

## Testing locally

Follow the [Material for MKDocs instructions](https://squidfunk.github.io/mkdocs-material/getting-started/)

```
$ git clone https://github.com/cyverse-learning-materials/container-camp.git
$ cd container-camp
$ pip install mkdocs-material
$ mkdocs serve
```

## Action with ReadTheDocs Theme

This is a template that uses the [MkDocs deploy](https://github.com/marketplace/actions/deploy-mkdocs) GitHub action.

We are using the `@nomaterial` branch for the [Action](.github/workflows/main.yml) to produce the ReadTheDocs style layout with the `theme: readthedocs` in the [mkdocs.yml](./mkdocs.yml):

```
theme:
  name: readthedocs
```

## Action with Material Theme

To change to [MkDocs Material](https://squidfunk.github.io/mkdocs-material/) theme, change [Action](./github/workflows/main.yml) to `@master` and set `theme: material` in the [mkdocs.yml](./mkdocs.yml):

```
theme:
  name: material
```
