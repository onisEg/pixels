# Pixels · Creative Agency

A single-page creative agency exercise built with HTML, CSS and local imagery. The project demonstrates a float-based approach to composing a portfolio page.

[Open the live demo](https://oniseg.github.io/pixels/) · [View screenshot](https://raw.githubusercontent.com/onisEg/resume/23df91e50f87b60e1360d79edcc24cf77eb09b07/public/projects/pixels.webp)

## Page structure and layout

1. The hero introduces the agency, followed by a featured-work section. About, Services and Reviews continue on the same document.
2. The featured and about sections share the `featured` class. A change to that class can therefore affect both sections, even though their anchor IDs differ.
3. Several layout rules float elements left or right. When adding content, inspect the parent’s height and how the following section clears the previous row.

## Run locally

From the repository root, serve the checked-in files with Python 3:

```sh
python -m http.server 8000
```

Open [localhost:8000](http://localhost:8000/) to load `index.html`. The browser reads the HTML, styles and assets directly. On Windows, `py -m http.server 8000` starts the same server.

## Source guide

| File or directory | What to look for |
| --- | --- |
| [index.html](index.html) | Section sequence and the featured, about, services and contact anchors. |
| [style.css](style.css) | Column widths, floats, alignment and typography. |
| [imgs](imgs) | Agency images referenced by HTML and CSS. |

## Manual walkthrough

Open the page at the featured anchor and follow the navigation down to Services. Resize the viewport and look for horizontal overflow, clipped images or a following section overlapping a floated row. Use those checks when editing column widths.
