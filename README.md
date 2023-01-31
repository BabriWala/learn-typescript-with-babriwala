What is TypeScript?

Typescript is programming language. Powered by Mirosoft.
Typescript is Javascript with type supports.

Why TypeScript?

Avoid Bugs In Development - When we write js code in that we can't find any error but when we run this code in production we find many bugs with the hlp of typeScript we can find bug when we write the code.

Increase Development Speed - When we write js code with typescript we have to write extra code but this is better.

Additional Feature - enams, property modifies, interfaces which is  not available on javaScript

We cannot run typescript in production but we write code with the help of typescript .
But the mecanism is the typescript code converted into js 

Install TypeScript

For install typescript you have to have nodejs and if you don

npm install -g typescript
-g this mean i can access this package from anywhere in my computer

tsc --help for more details about typescript

// js code 

// here we can see that a variabele that has string doing arithmetic operation with number that will create concatinating and this problem only show whent it goes to production

let num1 = '1'
function calculate (num1, num2){
return num1 + num2;
}

// this will output = 12 but the actual output is 3 and overcome this problem we have typescript
console.log(calculate(num1, 2))


// now we will see how typescript help us to overcome this problem 
// Here we tell that in calculate arguments that num1 and num2 will be only number type that's why now this will give us an error for assigning string to a number type value

let num1 = '1'
function calculate (num1 : number, num2 : number ){
return num1 + num2;
}

console.log(calculate(num1, 2))
