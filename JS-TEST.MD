### Sum of several arrays

    You will be given an array of several arrays that each contain integers and your goal is to write a function that will sum up all the numbers in all the arrays. For example, if the input is [[3, 2], [1], [4, 12]] then your program should output 22 because 3 + 2 + 1 + 4 + 12 = 22.


    function sum_array(arr) {
      
      // store our final answer
      var sum = 0;
      
      // loop through entire array
      for (var i = 0; i < arr.length; i++) {
        
        // loop through each inner array
        for (var j = 0; j < arr[i].length; j++) {
          
          // add this number to the current final sum
          sum += arr[i][j];
          
        }
        
      }
      
      return sum;
      
    }

    sum_array([[3, 2], [1], [4, 12]]);

  


### Determine overlapping numbers in ranges

    You will be given an array with 5 numbers. The first 2 numbers represent a range, and the next two numbers represent another range. The final number in the array is X. The goal of your program is to determine if both ranges overlap by at least X numbers. For example, in the array [4, 10, 2, 6, 3] the ranges 4 to 10 and 2 to 6 overlap by at least 3 numbers (4, 5, 6), so your program should return true.


    function OverlappingRanges(arr) {

      // keep a count of how many numbers overlap
      var counter = 0;
      
      // loop through one of the ranges
      for (var i = arr[0]; i < arr[1]; i++) {

        // check if a number within the first range exists
        // in the second range
        if (i >= arr[2] && i <= arr[3]) { 
          counter += 1;
        }

      }
     
      // check if the numbers that overlap is equal to or greater
      // than the last number in the array
      return (counter >= arr[4]) ? true : false;
    }

    OverlappingRanges([4, 10, 2, 6, 3]); 



### First Factorial

    Have the function FirstFactorial(num) take the num parameter being passed and return the factorial of it (ie. if num = 4, return (4 * 3 * 2 * 1)). For the test cases, the range will be between 1 and 18. 


    function FirstFactorial(num) { 
      var x = 1;
      for (var i = 1; i <= num; ++i){
        x *= i
      };
      return x;
    }

    FirstFactorial(18);   


### Longest word

    Have the function LongestWord(sen) take the sen parameter being passed and return the largest word in the string. If there are two or more words that are the same length, return the first word from the string with that length. Ignore punctuation and assume sen will not be empty. 


    function LongestWord(sen) { 
      var words = sen.split(" ").sort(function(a,b){
        return b.replace(/[^a-z]/gi,"").length - a.replace(/[^a-z]/gi,"").length;
      });
      return words.shift();
    }






