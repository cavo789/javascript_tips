# javascript_tips

> Some tips &amp; tricks and snippets for javascript.

* [Snippets](#snippets)
  * [Change color of links when clicked](#change-color-of-links-when-clicked)
* [Author](#author)
* [License](#license)

## Snippets

### Change color of links when clicked

When a link has been clicked, change his style to make simple to visualize un visited links.

Prefer js and not css (`a:visited {color: cyan; }`) so we can simply refresh the page (JS) without having to clear the browser history (css).

Idea is to be able to detect on a page which links have been clicked.

```javascript
<script>
document.addEventListener("DOMContentLoaded", () => {
    (
        addEventListener('click', function (ev) {
            ev.target.style.color = 'cyan';
        })
    )
});
</script>
```

## Author

Christophe Avonture

## License

[MIT](LICENSE)
