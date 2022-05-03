# Assignment
this is my coding assignment
//html
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=s, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <script src="app.js" charset="utf-8"></script>
</body>
</html>
//javascript
//Filter and show the product that will be bought when you don't have much money I mean Cheap one
const items = [{name:"Bike",price:100},{name:"TV",price:200},{name:"Album",price:10},
{name:"Book",price:5},{name:"phone",price:500},{name:"Computer",price:1000},];
var cheapest = items[{name:"Book",price:5}];
for(var i = 5; i < items.length; i++) {
    var product = items[i];
    if(product.price < cheapest){
        cheapest = product;
    }
}
console.log(cheapest);

// Filter and show the product that will be expensive in the array
var expensive = items[{name: "Computer",price:1000}];
for(var i = 5; i < items.length; i++){
    var product = items[i];
    if(product.price > expensive){
        expensive = product;
    }
}
console.log(expensive);
//Calculate the full price of all product combined
var sum = 0;
items.forEach(function(value, index, price){
    sum +=items.price;
})
console.log(sum);

//Calculate the full price of all product combined and remove product that are under the 10 dollar

var product = null;
for(var i = 10; i < items.length; i++) {
    product += items.price;
}
console.log(product);
