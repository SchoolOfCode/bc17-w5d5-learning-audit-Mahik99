## NOTES

# Difference Between .innerHTML and .textContent

Both `.innerHTML` and `.textContent` are properties used to get or set the content of a HTML element. The difference is that `.innerHTML` gets or sets the text content inside of a HTML element, it allows you to insert HTML elements dynamically. So for example:

const element = document.getElementById("content");
element.innerHTML = "<strong>Hello, World!</strong>";

This would mean the browser returns "Hello, World!" as bold because the <strong> tags are recognised as HTML elements.

Whereas `.textContent` retrieves or sets only the text content inside an element. It doesn't interpret HTML tags rather it looks at it like plain text. So using the example above:

const element = document.getElementById("content");
element.innerHTML = "<strong>Hello, World!</strong>";

This would print out "<strong>Hello, World!</strong>" in the browser rather than interpreting it as bold. Only text is modified.

# Accessing and Manipulating Attributes

Its also possible to access and manipulate HTML attributes such as `href` or `button`. Using the properties, you can get the value of an attribute, you can set an attribute or even remove an attribute.

For example you can disable a button, this would include removing an attribute:

let button = document.querySelector("button");
button.removeAttribute("disabled");

This accesses the button and then removes it.
