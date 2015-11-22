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
