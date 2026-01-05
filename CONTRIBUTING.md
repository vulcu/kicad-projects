# Contributing

All contributions require a pull request. Only rebase merges are supported.

## Getting Started

This project is built with KiCad 9.0 or later.

Recommended: Install [KiCad 9.0](https://github.com/KiCad/kicad-source-mirror/blob/master/INSTALL.txt)
and use to install the latest KiCad version.

Clone the repository to the directory of your choice
```sh
git clone git@github.com:vulcu/kicad-projects.git
```

### Install Dependencies

After cloning the repo, directory you cloned it to and run the following to
install schematic and footprint library dependencies

```sh
git clone git@github.com:vulcu/kicad-library.git
```

### Linting

PRs will not merge if they fail linting.
To confirm linting locally, run:

```sh
# linting is not currently enforced for this project
```

### Install Global Libraries

- Open KiCad, and select the Symbol-Editor. Select 'File >> Add Library' and select 'Global' when prompted. Navigate to the `kicad-library/symbol' directory and select `vulcu.kicad_sym`.
- Open KiCad, and select the Symbol-Editor. Select 'File >> Add Library' and select 'Global' when prompted. Navigate to the `kicad-library/footprint' directory and select the `vulcu.pretty` directory.

This command will watch for changes and update the local
server automagically.

## Projects

This repository includes the following projects:

- isolation-transformer
- captouch-keyboard

## Adding files

All KiCad project files should be added to the relevant project directory, aka `kicad-projects/[project]`.

### Documentation

- Add MCAD data to `kicad-projects/[project]/mcad/[file-name][-##].jpg`
- Written documentation should be in the form of `*.md` markdown files conforming this [style guide](https://google.github.io/styleguide/docguide/style.html)

### MCAD Data and 2D/3D Mockups

- Add MCAD data to `kicad-projects/[project]/mcad/[file-name][-##].jpg`
- MCAD data does not have to be optimized, and can be up to 100 MB per file. Large files (>25 MB) should be compressed using standard, unencrypted `*.gzip` or `*.7z` archive files if possible.

### Including Images

Images do not have to be optimized, however they should be of a reasonable filesize (2-5 MB is ideal).

You can add as many images as you like. The first image will be used as
the featured image at the top of the recipe and as the thumbnail image.

- Add images to `kicad-projects/[project]/images/[image-name][-##].jpg`
- Each image must have [alt text](https://www.w3.org/WAI/tutorials/images/informative/#example-2-images-used-to-supplement-other-information).
- Images may optionally have a photographer, source, and/or [license](https://spdx.org/licenses/).

### Required and Optional Details
