# GitHub CLI

`gh` es GitHub en la línea de comandos. Trae solicitudes de extracción, problemas y otros conceptos de GitHub al terminal junto a donde ya está trabajando con `git` y su código.

![screenshot of gh pr status](https://user-images.githubusercontent.com/98482/84171218-327e7a80-aa40-11ea-8cd1-5177fc2d0e72.png)

La CLI de GitHub está disponible para repositorios alojados en GitHub.com y GitHub Enterprise Server 2.20+, y para instalar en macOS, Windows y Linux.

## Documentation

[See the manual][manual] para obtener instrucciones de configuración y uso.

## Contributing

Si algo se siente mal, o si cree que falta alguna funcionalidad, consulte la [contributing page][contributing]. Allí encontrará instrucciones para compartir sus comentarios, crear la herramienta localmente y enviar solicitudes de extracción al proyecto.

<!-- this anchor is linked to from elsewhere, so avoid renaming it -->
## Instalacion

### macOS

`gh` está disponible a través de [Homebrew] [], [MacPorts] [], [Conda] [], [Spack] [], y como binario descargable desde la [página de lanzamientos] [].

#### Homebrew
| Install:          | Actualizacion         |
| ----------------- | ----------------- |
| `brew install gh` | `brew upgrade gh` |

#### MacPorts

| Install:               | Actualizacion                                       |
| ---------------------- | ---------------------------------------------- |
| `sudo port install gh` | `sudo port selfupdate && sudo port upgrade gh` |

#### Conda

| Install:                                 | Upgrade:                                |
|------------------------------------------|-----------------------------------------|
| `conda install gh --channel conda-forge` | `conda update gh --channel conda-forge` |
Opciones adicionales de instalación de Conda disponibles en el [gh-feedstock page](https://github.com/conda-forge/gh-feedstock#installing-gh).
#### Spack

| Install:           | Upgrade:                                 |
| ------------------ | ---------------------------------------- |
| `spack install gh` | `spack uninstall gh && spack install gh` |

### Linux & BSD

`gh` esta disponible en  [Homebrew](#homebrew), [Conda](#conda), [Spack](#spack), puede ser descargado en [releases page][].

Para obtener instrucciones sobre distribuciones específicas y administradores de paquetes, consulte[Linux & BSD installation](./docs/install_linux.md).

### Windows

`gh` esta disponible en [WinGet][], [scoop][], [Chocolatey][], [Conda](#conda), and as downloadable MSI.

#### WinGet
| Instalacion:            | Actualizacion:            |
| ------------------- | --------------------|
| `winget install gh` | `winget upgrade gh` |

#### scoop

| Instalacion:           | Actualizacion:           |
| ------------------ | ------------------ |
| `scoop install gh` | `scoop update gh`  |

#### Chocolatey

| Instalacion:           | Actualizacion:           |
| ------------------ | ------------------ |
| `choco install gh` | `choco upgrade gh` |
#### Signed MSI

Los instaladores de MSI están disponibles para descargar en el[releases page][].

### GitHub Actions

GitHub CLI viene preinstalado en todos [GitHub-Hosted Runners](https://docs.github.com/en/actions/using-github-hosted-runners/about-github-hosted-runners).

### Other platforms

Descargue los binarios empaquetados del [releases page][].

### Build from source

Vea aquí cómo [build GitHub CLI from source][build from source].

## Comparison with hub

Durante muchos años, [hub] [] fue la herramienta CLI de GitHub no oficial. `gh` es un nuevo proyecto que nos ayuda a explorar
cómo puede verse una herramienta CLI oficial de GitHub con un diseño fundamentalmente diferente. Mientras tanto
las herramientas llevan GitHub a la terminal, `hub` se comporta como un proxy de` git`, y `gh` es independiente
herramienta. Consulte nuestra [explicación más detallada] [gh-vs-hub] para obtener más información.
[manual]: https://cli.github.com/manual/
[Homebrew]: https://brew.sh
[MacPorts]: https://www.macports.org
[winget]: https://github.com/microsoft/winget-cli
[scoop]: https://scoop.sh
[Chocolatey]: https://chocolatey.org
[Conda]: https://docs.conda.io/en/latest/
[Spack]: https://spack.io
[releases page]: https://github.com/cli/cli/releases/latest
[hub]: https://github.com/github/hub
[contributing]: ./.github/CONTRIBUTING.md
[gh-vs-hub]: ./docs/gh-vs-hub.md
[build from source]: ./docs/source.md
