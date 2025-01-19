# CSS Specificity Bug

This repository demonstrates an uncommon bug related to CSS selector specificity. The bug involves unexpected behavior due to the precedence of selectors.

## Bug Description

The CSS code contains two rules targeting `<p>` elements. One rule targets paragraphs within a `div` element (`div p`), while another targets all paragraphs (`p`). Due to the way CSS specificity works, the more specific selector (`p`) overrides the less specific selector (`div p`), leading to unintended styling.

## Bug Solution

The solution involves understanding and correctly applying CSS specificity rules. The solution uses the `!important` flag to correctly style the `<p>` element within a `div` element, overriding the `p` selector.

## How to Reproduce

1.  Clone the repository.
2.  Open `index.html` in your web browser.
3.  Observe that all paragraphs are styled with red text, even those inside the `div` element. This is the unexpected behavior due to specificity.