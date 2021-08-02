Write an algorithm that determines wether all the elements in a string are unique
dont use arrays or array methods

input: string
output: boolean

Input: "yes"
output: true

input: "food"
output: false

///"fod hel fa".charAt(0) = f
///string[0] === f

const isStringUnique = (inputtedString) => {
  for(var i=0;i<inputtedString.length;i++) {
    if(input[i] != " ") {
    for(var j=i+1;j<inputtedString.length;j++) {
        if (input[i] === input[j]) {
            return false;
        }
    }
    }
  }
  return true;
}

const input = "food";
isStringUnique(input);
