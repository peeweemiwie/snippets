# javascript snippets

## for loop to increment variable to build a timer

    var count = 10;
    var counterIncrement=-1;
    var counter = setInterval(timer, 500); 


    function timer() {
      count = count+counterIncrement;
          if (count == 0 || count == 10 ) {
            counterIncrement = -counterIncrement;
        }
      console.log(count);
    }


## forEach addEventListener

        var circles = d.querySelectorAll('.circle');
        [].forEach.call(circles, function(el){
                el.addEventListener('click', function(e){      
                        // DO SOMETHING I SAID!!!! 
                });
        });
        
        
        
## remove placeholder on focus

        var d = document;
        var tableInput = d.querySelectorAll('.margin-calc-table input');  
        [].forEach.call(tableInput, function(el){
                var placeholderVal = el.placeholder;
                el.addEventListener('focus', function(e){
                        el.placeholder = '';
                });
                el.addEventListener('blur', function(e){
                        el.placeholder = placeholderVal;
                });
        });



##insertAdjacentHTML

    element.insertAdjacentHTML(position, text);

https://developer.mozilla.org/en-US/docs/Web/API/Element/insertAdjacentHTML

##insertedNode

    var insertedNode = parentNode.insertBefore(newNode, referenceNode);

https://developer.mozilla.org/en-US/docs/Web/API/Node/insertBefore

##Node.insertBefore()

https://developer.mozilla.org/en-US/docs/Web/API/Node/insertBefore

    var insertedNode = parentNode.insertBefore(newNode, referenceNode);

  // Get a reference to the element in which we want to insert a new node
  
  `var parentElement = document.getElementById('parentElement');`
  
  // Get a reference to the first child
  
  `var theFirstChild = parentElement.firstChild;`

  // Create a new element
  
  `var newElement = document.createElement("div");`

  // Insert the new element before the first child
  
 `parentElement.insertBefore(newElement, theFirstChild);`

##toggle class

    function a(){
        this.classList.toggle('first');
        this.classList.toggle('sec');
    }
