+++
title = "Enable LaTeX math rendering?"
author = ["i0z0m"]
date = 2017-07-13T17:31:56-04:00
draft = false
markup = "pandoc"
+++

## setting in hugo {#setting-in-hugo}

> config/\_default/params.toml の math オプションを切り替え
> かつ Front Matter に markup: mmark を追加する。
> [Hugo での文章の書き方](https://sigu1011.github.io/post/how%5Fto%5Fwrite%5Fcontents/)

`config/_default/params.toml`

```nil
# Enable LaTeX math rendering? true/false
#   If false, you can enable math on a per page basis as needed.
math = true
```


## math with ox-hugo {#math-with-ox-hugo}

<https://gohugo.io/content-management/formats/#list-of-content-formats>

```nil
:EXPORT_HUGO_CUSTOM_FRONT_MATTER: :markup pandoc
```

<https://ox-hugo.scripter.co/doc/equations/>

LaTeX formatted equation: \\( E = -J \sum\_{i=1}^N s\_i s\_{i+1} \\)

\begin{equation}
\label{eq:1}
C = W\log\_{2} (1+\mathrm{SNR})
\end{equation}
