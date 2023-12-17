# Devicons Extension for Quarto

This extension provides support for
[devicons](https://devicon.dev). Icons can be used in
HTML documents only.

The code is adapted from the [academicons](https://github.com/schochastics/academicons) extension.

## Installing

```bash
quarto install extension schochastics/devicons
```

This will install the extension under the `_extensions` subdirectory.
If you're using version control, you will want to check in this directory.

## Using

To embed an icon, use the `{{{< devicon >}}}` shortcode. For example:

```default
{{< ai python-plain-wordmark >}} 
{{< ai cplusplus-plain >}}
{{< ai lua-plain-wordmark }}
{{< ai lua-plain-wordmark size=5x >}}
```

You can browse all of the available icons here:

<https://devicon.dev>

### Sizing Icons

This extension provides relative, literal, and LaTeX-style sizing for icons.  
When the size is invalid, no size changes are made.

- Relative sizing: `{{< ai lua-plain-wordmark size=2xl >}}`.

  | Relative Sizing Class | Font Size | Equivalent in Pixels |
  |-----------------------|-----------|----------------------|
  | 2xs                   | 0.625em   | 10px                 |
  | xs                    | 0.75em    | 12px                 |
  | sm                    | 0.875em   | 14px                 |
  | lg                    | 1.25em    | 20px                 |
  | xl                    | 1.5em     | 24px                 |
  | 2xl                   | 2em       | 32px                 |

- Literal sizing: `{{< devicon lua-plain-wordmark size=5x >}}`.

  | Literal Sizing Class | Font Size |
  |----------------------|-----------|
  | 1x                   | 1em       |
  | 2x                   | 2em       |
  | 3x                   | 3em       |
  | 4x                   | 4em       |
  | 5x                   | 5em       |
  | 6x                   | 6em       |
  | 7x                   | 7em       |
  | 8x                   | 8em       |
  | 9x                   | 9em       |
  | 10x                  | 10em      |

- LaTeX-style sizing: `{{< ai open-access size=Huge >}}`.

  | Sizing Command                   | Font Size (HTML) |
  | -------------------------------- | ---------------- |
  | tiny (= `\tiny`)                 | 0.5em            |
  | scriptsize (= `\scriptsize`)     | 0.7em            |
  | footnotesize (= `\footnotesize`) | 0.8em            |
  | small (= `\small`)               | 0.9em            |
  | normalsize (= `\normalsize`)     | 1em              |
  | large (= `\large`)               | 1.25em           |
  | Large (= `\Large`)               | 1.5em            |
  | LARGE (= `\LARGE`)               | 1.75em           |
  | huge (= `\huge`)                 | 2em              |
  | Huge (= `\Huge`)                 | 2.5em            |

- CSS-style sizing: `{{< ai open-access size=2em >}}`.

### Coloring icon

The color of the icon can be changed via the `color` parameter.  
`{{< ai open-access color=red >}}`


## Example

Here is the source code for a minimal example: [example.qmd](example.qmd)
