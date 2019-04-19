# some try on sass

nice website about this: <br/>
https://sass-guidelin.es/ <br/>
https://sass-lang.com/documentation/

## Bigger Projects

**For a bigger project, multiple page app, I use 7–1 pattern, it is similar to the small project file structure but with more folders. Here’s what 7–1 the pattern looks like.**
<br/>
- base/         ex: reset, typography
- components/   ex: nav, grod, header, footer, sidebar, forms
- layout/       ex: button, carousel, cover, dropdown
- pages/        ex: home, contact (can be squiz if not specific pages style)
- themes/       ex: theme, admin (can be squiz //)
- abstracts/    ex: variable, function, mixins, placeholders
- vendors/      ex: bootstrap, jquery-ui
- main.scss

**The base, components, and layout do the same job as the file structure above. However, instead of a single file, we now manage them in a folder.**
<br/>
- Base: animations, base, typography, and utilies.
- Components: have a single scss file for each individual component
- Layout: Header, footer, grid, navigation
- Pages: Have a single scss for each specific page
- Themes: deals with various themes (optional, I haven’t use it yet)
- Abstracts: handles function, mixins, and variables
- Vendor: handles 3rd party css
- Here’s a boilerplate from the original author.
<br/>

### Basic tips!
Nice general guide from here: https://sass-lang.com/guide 

### @mixin or @extend?
Only use @extend when the rulesets that you are trying to DRY out are inherently and thematically related. Do not force relationships that do not exist: to do so will create unusual groupings in your project, as well as negatively impacting the source order of your code.
<br/>
Use a mixin to either inject dynamic values into repeated constructs, or as a Sassy copy/paste which allows you to repeat the same group of declarations throughout your project whilst keeping a Single Source of Truth.