function printInfo( name, age){
    console.log(`${name}'s age is ${age}`);
}
printInfo("rahul", 32);

function sum(a,b){
    console.log(a+b);
}
sum(59,32);# Function


function printTable(n){
    for(i=n; i<=n*10; i+=n){
        console.log(i);
    }
}
printTable(49);

function getSum(n){
    let sum=0;
    for(i=0; i<=n; i++){
        sum+=i;
    }
    return sum;
}

let str=["hi", "hello", "bye", "!"];
result="";
function concat(){
    for(i=0; i<str.length; i++){
        result+=str[i];
    }
    return result;
}

function multipleGreet(func, n){
    for(i=0; i<=n; i++){
        func();
    }
}
greet=function() {
    console.log("namaste");
}
multipleGreet(greet, 8);

//Higher order which returns function

function oddOrEvenFactory(request){
    if(request=="even"){
        return function(n){
            console.log(n%2==0);
        }
    }
    else if(request=="odd"){
        return function(n) {
            console.log(!(n%2==0));
        }
    }
}
request="even"; 
