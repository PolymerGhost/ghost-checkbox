Polymer Ghost Checkbox
======================

Polymer ghost-checkbox uses the Polymer paper-checkbox component as a wrapper 
for the traditional HTML checkbox input.

Ghost-checkbox uses the underlying input to retrieve and store the checked 
value, so it can be easily used without changing any of the existing application
logic.

## Usage

To use it, simply wrap the existing checkbox input element in the ghost-checkbox
 tags:

```html
<ghost-checkbox>
    <label>
    	<input type='checkbox' name='hello' checked='checked' />
    	This is a label
	</label>
</ghost-checkbox>
```

```html
<ghost-checkbox>
    <input type='checkbox' name='hello' id='hello' checked='checked' />
    <label for='hello'>This is a label</label>
</ghost-checkbox>
```

Ghost-checkbox will recognize and take on the input's checked state and label.
It inherits directly from paper-checkbox, so it can be styled according to the 
instructions for styling paper-checkbox:

https://www.polymer-project.org/docs/elements/paper-elements.html#paper-checkbox

## Browser compatibility

Ghost-checkbox can be safely used with older browsers that don't support web 
components. The unsupported browsers will simply render the underlying checkbox
element.
