# web-components-aria-modal

Accessible modal with Web Components

# Install(ESM)

- `yarn add web-components-aria-modal` or `npm i web-components-aria-modal`

# Install(UMD)

- Please download the following code.
- https://unpkg.com/web-components-aria-modal@latest/dist/index.umd.js

# Usage

```js

import 'web-components-aria-modal';

/**
 * do something
*/

```

# Append Your Modal

You can append your modal inside aria-modal with `slot`. If you use `slot`, you can use accessible feature for modal.  
Please see following example.

```html

<aria-modal>
  <div name="modal">
    <!-- ... -->
  </div>
</aria-modal>

```

# Style

Using css variables, you can apply your style to `<aria-modal>`.

```css

aria-modal {
  --backdrop-display: block; /* or flex, inline-block, etc... */
  --backdrop-color: rgba(0, 0, 0, 0.3); /* background-color for backdrop */
  --backdrop-position: absolute; /* or fixed */
}

```

# Props

| name | required | default | description |
| :--: | :------: | :-----: | :--------- |
| `open` | `false` | `false` | It is used to show modal. You can set true if you want to open modal. |
| `first-focus` | `true` | *none* | It is used to focus to first element when modal is opened. You should assign id name. | 
| `node` | `true` | *none* | It is used to move focus inside modal. You should set modal id name. |
| `animation` | `false`| `false` | Fade animation will run if animation flag is true. |
| `duration` | `false` | `300` | animation duration time |
| `aria-label` or `aria-labelledby` | `true` | *none* | See https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/ARIA_Techniques/Using_the_aria-labelledby_attribute |
| `aria-describedby` | `true` | *none* | See https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/ARIA_Techniques/Using_the_aria-describedby_attribute |
| `role` | `true` | *none* | Assignable value are `dialog` or `alertdialog`. See https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles |
| `aria-modal` | `false` | `true` | See https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/dialog_role

# Example

https://github.com/github/clipboard-copy-element/tree/master/examples
