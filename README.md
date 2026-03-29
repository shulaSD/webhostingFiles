# webhostingFiles

A repository for hosting web assets (fonts, CSS, etc.) for use across websites.

## Fonts Directory

The `/fonts` folder contains web fonts in **woff** and **woff2** formats.

### How to Use Fonts

1. **Add your font files** to the `/fonts` folder (drag and drop into the folder)
2. **Use the `fonts.css`** file as a template to create `@font-face` declarations
3. **Reference fonts in your website** using the raw GitHub URLs:
   ```
   https://raw.githubusercontent.com/shulaSD/webhostingFiles/main/fonts/[filename].woff2
   https://raw.githubusercontent.com/shulaSD/webhostingFiles/main/fonts/[filename].woff
   ```

### CSS Example

```css
@font-face {
    font-family: 'MyFont';
    src: url('https://raw.githubusercontent.com/shulaSD/webhostingFiles/main/fonts/my-font.woff2') format('woff2'),
         url('https://raw.githubusercontent.com/shulaSD/webhostingFiles/main/fonts/my-font.woff') format('woff');
}

body {
    font-family: 'MyFont', sans-serif;
}
```

## Current Structure

```
webhostingFiles/
├── README.md
├── fonts.css
└── fonts/
    └── (add your .woff and .woff2 files here)
```
