# Javascript30 #1: JS Drum Kit

### The `<kbd>` Tag
The `<kbd>` tag is used to denote a keyboard input. User agents (browser) generally style this as monospace code-like text.
It can be nested for multi-key commands:
```
Copy: <kbd><kbd>Ctrl</kbd>+<kbd>c</kbd></kbd>
Paste: <kbd><kbd>Ctrl</kbd>+<kbd>v</kbd></kbd>
```
> Copy: <kbd><kbd>Ctrl</kbd>+<kbd>c</kbd></kbd>
> Paste: <kbd><kbd>Ctrl</kbd>+<kbd>v</kbd></kbd>

### The `data` Attribute
- Provides the ability to embed custom attributes to HTML elements using the prefix 'data-'

### `Element.classList`
- a read-only property which returns a live DOMTokenList collection of the class attributes of the element.
- Using classList is a convenient alternative to accessing an element's list of classes as a space-delimited string via element.className
- Methods:
    - .add('string') adds specified classes. If they exist already they are ignored
    - .remove('string') removes specific class, does not throw an error if class doesn't exist
    - .item(number) Return class value by index provided
    - .toggle() remove class if it exists, add class if it doesn't
    - .contains(string) returns if class exists or not
    - .replace(oldClass, newClass) replace one class with another

### `docuemnt.querySelector(selector)`
- Returns the first element that matches the `selector`
- `selector` must be a valid CSS selector:
    - `document.querySelector(".myclass")`
    - `document.querySelector("div.user-panel.main input[name='login']")`

### `document.querySelectorAll(selector)`
- Returns a static (not live) NodeList representing a list of the document's elements that match the specified group of selectors.
