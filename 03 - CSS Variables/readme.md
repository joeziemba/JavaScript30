# 03 CSS Variable Notes

## CSS Variables
- Different than Scss variables
- Can be updated with Javascript

#### Declaration:
```
:root {
  --base-color: #ffc600;
  --spacing: 10px;
  --blur: 10px;
}
```
  - The `:root` CSS pseudo-class matches the root element of a tree representing the document. In HTML, :root represents the `<html>` element and is identical to the selector html, except that its specificity is higher. It can also be used to declare CSS variables.
  - The double hyphen is required for variables

#### Usage:
CSS Variables are accessed using the `var()` function
```
h1 {
  color: var(--base-color)
}
```

#### Changing a variable:
```
function handleUpdate() {
  document.documentElement.style.setProperty(`--${this.name}`, this.value);
}
```

## `dataset` with `document.querySelectorAll`
Dataset is an object that contains all custom `data-` properties as key-value pairs.
