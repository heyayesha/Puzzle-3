# Puzzle-3
//  Write a function in Javascript that will reverse every word in a given string and return the new string. Every word should be reversed but the string as a whole // should not be reversed. And DO NOT use array.reverse() method


function reverseStrWords(str){

  let myArr = str.split("");      //each work is put from string into an array
  let tempArr = [];              // to new array with words reversed 
  let tempWord ="";             // this will will hold the reversed string 
  let word ="";                // here place holder for the index of the current string index

  //LOOPS through array from end
  
  for(let i = myArr.length-1; i >= 0; i--){

      word = myArr[i];       //holds word at current index

//Loops through each char of the word from the end

    for(let j = word.length - 1; j >= 0; j-- ){

      tempWord += word.charAt(j);    //builds reverse string 

    }

  }
    tempArr.push(tempWord);      //adds revered string to array 
    return tempArr.join("");    //turns the array back into a string
}
