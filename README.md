# LaTeX Notes Template

Overleaf template for research notes. Upload `main.tex`, `mystyle.sty`, and `citations.bib` to a new Overleaf project.

## Files

- `main.tex` — document skeleton with geometry, packages, and a starter `emphbox` for overarching questions
- `mystyle.sty` — custom package: color palette, code listings style, and semantic callout boxes
- `citations.bib` — BibTeX references

## Custom boxes (from `mystyle.sty`)

| Environment | Purpose |
|---|---|
| `emphbox` | General-purpose callout (no numbering) |
| `questionbox` | Specific questions, numbered per section |
| `confusionbox` | Things that are unclear or uncertain |
| `rqbox` | Research questions |
| `hypothesisbox` | Hypotheses |
| `experimentbox` | Planned or completed experiments |
| `resultbox` | Empirical findings |
| `\commentbox[Initials]{...}` | Commentary with optional attribution |

## Usage

```latex
\begin{rqbox}{TITLE}
  Does tokenization choice affect downstream task performance?
\end{rqbox}

\begin{experimentbox}{}
  Train two models differing only in tokenizer; compare perplexity and few-shot accuracy.
\end{experimentbox}

\commentbox[GS]{Revisit after the ablation.}
```

Margin notes are available via `\marginnote{...}` from the `marginnote` package.
