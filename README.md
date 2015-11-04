# snippets

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



        var circles = d.querySelectorAll('.circle');
        [].forEach.call(circles, function(el){
                el.addEventListener('click', function(e){      
                        // DO SOMETHING I SAID!!!! 
                });
        });
