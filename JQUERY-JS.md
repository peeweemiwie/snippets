# jQuery to javascript

jQuery `.parent()` -> js `.parentNode`

jQuery `.siblings()` -> js `.parentNode.childNodes[]`

jQuery `.addClass()` -> js `.className = "new-class-name"` also `.classList.add("new-class-name")`

jQuery `.removeClass()` -> js `.className = ""` also `.classList.remove("class-name")`

jQuery `.hasClass()` -> js `.classList.contains("class-name")`

jQuery `.append()` -> js `.insertAdjacentHTML(position, text)` 

https://developer.mozilla.org/en-US/docs/Web/API/Element/insertAdjacentHTML

  * `beforebegin` Before the element itself.
  * `afterbegin` Just inside the element, before its first child.
  * `beforeend` Just inside the element, after its last child.
  * `afterend` After the element itself.

jQuery `.siblings()` -> js `.nextSibling`  `.nextElementSibling` 
