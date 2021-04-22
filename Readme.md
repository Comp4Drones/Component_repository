# Comp4Drones Component Repository

This repository aim at providing the D3.5: _Components repository_ associated with the task T3.3: _Generic components for drones_ of the [Comp4DRones](https://www.comp4drones.eu/) project.

Consult the website here: [https://comp4drones.github.io/Component\_repository/](https://comp4drones.github.io/Component_repository/)

This repository uses [MkDocs](https://www.mkdocs.org/) which allow to build static website from markdown files.

See the markdown syntax : [https://www.markdownguide.org/basic-syntax/](https://www.markdownguide.org/basic-syntax/)

## Contributing

Install MkDocs and the necessary requirements:

```
pip3 install -r requirements.txt
```

You can then render the site with your modifications by launching `mkdocs serve`.

You can also generate a PDF from it by setting the `C4D_PDF_EXPORT` environnement variable:

```
C4D_PDF_EXPORT=1 mkdocs build
```

See [MkDocs](https://www.mkdocs.org/) for more information.

