# Simple CodeEditor for Vue.js



Vue.js version: 3.0

website: [simple-code-editor.vicuxd.com](https://simple-code-editor.vicuxd.com)

It's easy to use, both support read-only and edit mode, you can directly use it in the browser or import the JavaScript modules via the NPM package



## Useage


Step 1

```shell
npm install simple-code-editor
```
Step 2. Importing the component and registration.
```javascript
import CodeEditor from 'simple-code-editor';
export default {
    components: {
      CodeEditor
    }
}
```
```html
<CodeEditor></CodeEditor>
```



#### Customizing the theme style

You can cover the CSS file to customize the theme style.

```html
<!--1. Setting the theme to an empty value-->
<!--2. Add your customized class to change the style-->
<CodeEditor theme="" class="github_dark"></CodeEditor>
```



## API

### read_only ` Boolean`

Default:  `false`

Description: whether the code is editable

```html
<CodeEditor :read_only="true"></CodeEditor>
```



### value `String`

Default:  `unset`

Description: setting the contents of a code editor. If you want to bind the data, please use the property [`v-model`](#v-model)

```html
<CodeEditor value="console.log(13)"></CodeEditor>
```



### v-model

Description: varies based on the value of form inputs element or output of components, the specific usage you can read [Vue.js Documentation](https://v3.vuejs.org/api/directives.html#v-model)




### language_selector `Boolean`

Default:  `false`

Description: whether the language selector is availed, if the value is `true`, you can use the property `languages` to set which languages can be selected

```html
<CodeEditor :language_selector="true"></CodeEditor>
```




### languages `Array`

Default: `[["javascript", "JS"],["cpp", "C++"],["python", "Python"]]`

Description: This property is a two-dimensional array, the first item of each child is an index of the language and it's required, the second item of each child is used for display, which is for the better user reading experience, it can be free to customize and optional, if it's unset, the UI display will be replaced with the index of the language. When the value of `language_selector` is `true`, you can set multiple languages to be selected

```html
<CodeEditor :language_selector="true" :languages="[['javascript', 'JS'],['python', 'Python']]"></CodeEditor>
```



### wrap_code  `Boolean`

Default:  `false`

Description: whether the code is allowed to wrap automatically

```html
<CodeEditor :wrap_code="true"></CodeEditor>
```



### hide_header  `Boolean`

Default:  `false`

Description: whether the header of code editor is hidden

```html
<CodeEditor :hide_header="true"></CodeEditor>
```



### display_language  `Boolean`

Default:  `true`

Description: whether the language name is displayed

```html
<CodeEditor :display_language="false"></CodeEditor>
```



### copy_code  `Boolean`

Default:  `true`

Description: whether the code can be copied by the icon button

```html
<CodeEditor :copy_code="true"></CodeEditor>
```



### theme `String`

Default:  `dark`

Description: switching between light and dark themes

```html
<CodeEditor theme="light"></CodeEditor>
```



### font_size  `String`

Default:  `17px`

Description: setting the font size

```html
<CodeEditor font_size="17px"></CodeEditor>
```



### width  `String`

Default:  `540px`

Description: setting the width of the code editor

```html
<CodeEditor width="540px"></CodeEditor>
```



### height  `String`

Default:  `auto`

Description: the height of the container is adaptive by default, you can also set it to a specific value, and the scroll bar will work with a long text

```html
<CodeEditor height="150px"></CodeEditor>
```



### min_width  `String`

Default:  `unset`

Description: setting the min-width of the code editor

```html
<CodeEditor min_width="200px"></CodeEditor>
```



### min_height  `String`

Default:  `unset`

Description: setting the min-height of the code editor

```html
<CodeEditor min_height="200px"></CodeEditor>
```



### max_width  `String`

Default:  `unset`

Description: setting the max-width of the code editor

```html
<CodeEditor max_width="200px"></CodeEditor>
```



### max_height  `String`

Default:  `unset`

Description: setting the max-height of the code editor

```html
<CodeEditor max_height="200px"></CodeEditor>
```



### border_radius  `String`

Default:  `12px`

Description: setting the radius of the code editor

```html
<CodeEditor border_radius="4px"></CodeEditor>
```



### selector_width  `String`

Default:  `110px`

Description: setting the width of the selector

```html
<CodeEditor selector_width="150px"></CodeEditor>
```



### selector_height  `String`

Default:  `auto`

Description: setting the height  of the selector

```html
<CodeEditor selector_height ="90px"></CodeEditor>
```



### selector_displayed_by_default   `Boolean`

Default:  `false`

Description: whether the selector is displayed by default

```html
<CodeEditor :selector_displayed_by_default="true"></CodeEditor>
```



### z_index   `String`

Default:  `unset`

Description: setting the stack order of the code editor

```html
<CodeEditor z_index="6"></CodeEditor>
```





