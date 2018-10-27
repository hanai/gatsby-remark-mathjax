# gatsby-remark-mathjax

[gatsby-remark-mathjax][1] adds mathjax support to gatsby using [remark-math][2].

## Install

`npm install --save gatsby-transformer-remark gatsby-remark-mathjax`

## How to use

```javascript
// In your gatsby-config.js
plugins: [
  {
    resolve: `gatsby-transformer-remark`,
    options: {
      plugins: [
        `gatsby-remark-mathjax`,
      ],
    },
  },
],
```

**Add MathJax to your template:** MathJax is required to render the formulas correctly. [MathJax: Getting Started](http://docs.mathjax.org/en/latest/start.html)

``` html
<script src='https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.5/MathJax.js?config=TeX-MML-AM_CHTML' async></script>
```

### Math Equations in Inline Mode

Surround your equation with `$` to generate a math equation in inline mode.

**Example markdown:**

```
$a^2 + b^2 = c^2$
```

### Math Equations in Display Mode

Surround your equation with `$$` and new-lines to generate a math equation in
display mode.

**Example markdown:**

```
$$
a^2 + b^2 = c^2
$$
```

[1]: https://github.com/hanai/gatsby-remark-mathjax
[2]: https://github.com/Rokt33r/remark-math
