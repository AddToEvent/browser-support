# Add to Event Browser Support

This repo has a centralised configuration for an Outdated Browser Banner, which can be used across the entire Add to Event ecosystem.

The goal of this repo is to create a centralised directory so everyone is supporting the same browsers across all Add to Event projects, existing and old.

It is just a customised version of the [Browser Update](https://browser-update.org/), with all the browsers we do / don't support.

### Summary of Browser Support

Main difficult contenders are old editions of IE. Most of our issues are solved with SCSS and a good autoprefixer. 

#### Supported
- Chrome (version 20 (discontinued by Google) or higher) – Browser pushes for upgrade, so we shouldn't need to.
- Opera (last 6 versions) – No known issues in lesser versions, but push for upgrade.
- Firefox (last 6 versions) – No known issues in lesser versions, but push for upgrade.
- Safari (last 3 versions) – No known issues in lesser versions, but push for upgrade.
- Edge (all versions)
- IE11.

#### Not Supported
- All browsers not included above.
- Below IE10 and below (Sites are expected to work in IE10, unofficially).

### Installation of Repo

Included in this repo are:
- `update-browser-min.js`
- `browser-update.css`
- `browser-update.scss`

Include and reference the js file in your HTML / PHP template or page. 

```
<script src="{ path to file }update-browser-min.js" async defer></script>
```


You can also just take the snippet and roll it into any existing JS. Best practice (and to catch errors) is to implement it *before* the page, just incase a JS error happens, which would prevent the banner loading. In reality, it is included as the last file, with `async defer` on the [Blog](https://blog.addtoevent.co.uk/), [Pro Centre](https://pro-centre.addtoevent.co.uk/), and [Careers](https://careers.addtoevent.co.uk/) site.