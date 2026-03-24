# LaTeX CV Template

A clean, modern, and highly customizable CV template based on the `curve` LaTeX class. This template is designed to be easy to use and looks great whether compiled with pdfLaTeX, XeLaTeX, or LuaLaTeX.

## Features

- **Modular Design**: CV sections are split into separate `.tex` files for easy management.
- **Publication Support**: Integrated `biblatex` support for highlighting your research and publications.
- **Social Icons**: Built-in support for `fontawesome5` and `simpleicons` for professional links (Email, GitHub, LinkedIn, etc.).
- **Photo Inclusion**: Optional profile photo support.
- **Cross-Engine Compatibility**: Works with pdfLaTeX, XeLaTeX, and LuaLaTeX.
- **Elegant Styling**: Custom headers, colored section markers, and beautiful typography.

## Prerequisites

To compile this CV, you will need a LaTeX distribution (like TeX Live, MiKTeX, or MacTeX). The following packages are primarily used:

- `curve` (the base class)
- `biblatex` (for publications)
- `fontawesome5` & `simpleicons` (for icons)
- `geometry` (for margins)
- `xcolor` & `tikz` (for styling)

## Usage

### 1. Customization

- **Main File**: Edit `cv-main.tex` to change your name, contact information, and which sections to include.
- **Sections**: Update the individual `.tex` files in the root directory:
  - `profile.tex`
  - `education.tex`
  - `employment.tex`
  - `skills.tex`
  - `publications.tex`
  - `misc.tex`
- **Styling**: Modify `settings.sty` to change colors, fonts, and layout parameters.
- **Publications**: Add your papers to `own-bib.bib`.

### 2. Compilation

You can compile the CV using your preferred engine. XeLaTeX or LuaLaTeX is recommended if you want to use specific OpenType fonts.

```bash
# Using latexmk (recommended)
latexmk -pdf -xelatex cv-main.tex

# Or manually with XeLaTeX
xelatex cv-main.tex
biber cv-main
xelatex cv-main.tex
```

## Preview

[Download/View PDF](cv-main.pdf)

![CV Preview](example.jpeg)

## License

This project is licensed under the GNU General Public License v3.0 (GPL-3.0) - see the [LICENSE](LICENSE) file for details.

### Acknowledgments
- Inspired by the work of [LianTze Lim](mailto:liantze@gmail.com).
- Modified and maintained by [Andrei Botez](mailto:andrei@straja.org).
