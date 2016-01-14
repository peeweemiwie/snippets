# css snippets

## box-sizing

    * {
      box-sizing: border-box;
    }

## rem calculation

    body { 
      font-size:62.5%; 
    }

## SCSS compass

    @include font-face("Blooming Grove", font-files("examples/bgrove.ttf", "examples/bgrove.otf"));
    .example {
      font-family: "Blooming Grove";
      font-size: 1.5em;
    }


## Style Input Placeholder

      ::-webkit-input-placeholder { /* WebKit, Blink, Edge */
         color:    #909;
      }
      
      :-moz-placeholder { /* Mozilla Firefox 4 to 18 */
         color:    #909;
         opacity:  1;
      }
      
      ::-moz-placeholder { /* Mozilla Firefox 19+ */
         color:    #909;
         opacity:  1;
      }
      
      :-ms-input-placeholder { /* Internet Explorer 10-11 */
         color:    #909;
      }
      
      :placeholder-shown { /* Standard (https://drafts.csswg.org/selectors-4/#placeholder) */
        color:    #909;
      }
