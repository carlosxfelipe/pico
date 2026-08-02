<p>
  <a href="https://picocss.com" target="_blank">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/picocss/pico/HEAD/.github/logo-dark.svg">
      <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/picocss/pico/HEAD/.github/logo-light.svg">
      <img alt="Pico CSS" src="https://raw.githubusercontent.com/picocss/pico/HEAD/.github/logo-light.svg" width="auto" height="60">
    </picture>
  </a>
</p>


# Preview
| Pico version | Tech stack |
| ----- | ----- |
| 2 | HTML, JavaScript |

A pure HTML example, without dependencies.


## Brand Color Mapping

- Pico 100: `#fcf2f2` (shade0)
- Pico 200: `#fbe9ea` (shade100)
- Pico 300: `#f6d1d2` (shade200)
- Pico 350: `#f2b6b7` (shade300)
- Pico 450: `#ee9b9d` (shade400)
- Pico 500: `#e96b6f` (shade500)
- Pico 600: `#e41e2b` (shade600)
- Pico 700: `#d01b27` (shade700)
- Pico 800: `#b61822` (shade800)
- Pico 850: `#a1151e` (shade900)
- Pico 900: `#841119` (shade1000)
- Pico 950: `#5d0c12` (shade1100)

## Additional Configurations

- `$enable-responsive-typography: false`: Disabled because Pico CSS default font sizes tend to be much larger than standard preferences. This keeps the typography more compact and consistent across different screen sizes.

## Updating CSS Themes

If you want to update the generated CSS files for this example, you need to adjust the build script located at `scripts/build-themes.js` in the root of the repository.

1. Ensure the output directory points to this example's `css` folder by modifying:
   ```javascript
   const cssFoldername = path.join(__dirname, "../examples/v2-html/css");
   ```

2. Specify which colors to generate by updating the colors array. For example, if you want to generate **only** the `brand` custom color, change it to:
   ```javascript
   const customColors = ["brand"];
   const themeColors = [...customColors];
   ```

3. Run the script from the root of the repository:
   ```bash
   node scripts/build-themes.js
   ```
