
=================================================

     Know Most Advanced Loop and Array task <Start>

=================================================
// problems

- reverse an array
- sum of array elements
- swap array elements
- Find Array elements
- Find Max/ Min number
- Filter an array
- using .find() .filter()
- calculating Discount 
- solving same problem using map/ foreach()
- Frequency array 
- Findout maximum occurance
- serial change

// kono kaj ekadikbar korar jonno loop use hoi

for ( let i = 0; i<5 ; i++){
    console.log(i)
}
// loop bebohar kore lav ki ?
// amra jani array 1st index number 0 hoi , aaray size ja hoi tar last index 1 kom hoi


// loop and array task //
// -----------------------------------------------------------------------
/// problems: 1///
/// forward loops with array
// decl array , dec for loops
// use log with arr name then [variable name (for)]

let arr = ['mango', 'grape', "pineapple", "guave", "melon"]

for (let i = 0; i<5 ; i++){
    console.log(arr[i]);       // forward loop // i=0 index mango ke nise, i=1 index grape ke nise aebabe choltese
}
// -----------------------------------------------------------------------
/// problems : 2 ///
/// Reversed loops with array
// use decrement thats it .

let arr = ['mango', 'grape', "pineapple", "guave", "melon"]

for (let i = arr.length-1 ; i>=0 ; i--){
    console.log(arr[i]);
}
// -----------------------------------------------------------------------

/// problems : 3 ///
/// sum of array element
let number = [10, 20, 30, 40, 50, 60]
let sum = 0
// i = 0 means it stating from 0 index , i<number.length means i<6
for(let i =0 ; i<number.length ; i++){ 
    const currentNUmber = number[i]
    sum = sum + currentNUmber
    console.log(sum);// ekdom ses sum i,e pura complete hole bosate cie , tiele console baire den
    //console.log(currentNUmber);
    //console.log(number[i]);
}
console.log(sum);
// -----------------------------------------------------------------------
// -----------------------------------------------------------------------

/// problems : 4 ///
/// substraction of array element
let numbers = [10, 20, 30, 40, 50, 60]
let substraction = 0
// i = 0 means it stating from 0 index , i<number.length means i<6

for ( let i = 0; i<numbers.length ; i++){
    let currentNumbers = numbers[i] // array theke number save kore seta variable e nicci e protibar
    substraction = currentNumbers - substraction
    
    //console.log(numbers[i]);
}
console.log(substraction);
// -----------------------------------------------------------------------


// -----------------------------------------------------------------------
/// problems : 6 ///
/// swap array elements
 let numbers = [10, 20, 30, 40, 50, 60]
// doren ami cie 1index 20 ; 3index 40 er jaigai jabe ; and 40 , 20 er jaigai jabe
// -----------------------------------------------------------------------

 let numbers = [10, 20, 30, 40, 50, 60]

let temp = numbers[3] // mone koren 40 harie jabe , taile save koren tare varible er modde
numbers[3]= 20; /// 3index er value change korsi
numbers[1]= temp // 1 index er value o change korsi , konta jeta ektu agge hariete niccilo
console.log(numbers);
-----------------------------------------------------------------------
let numbers = [10, 20, 30, 40, 50, 60]

let temp = numbers[5] // mone koren 60 harie jabe , taile save koren tare varible er modde
numbers[5]= 10; /// 5index er value change korsi, jehoto 10 60er jaiga replace korbe
numbers[0]= temp // 0 index er value o change korsi , konta jeta ektu agge hariete niccilo
console.log(numbers);

// -----------------------------------------------------------------------
/// problems : 7 ///
/// Find array elements
let fruits = ['mango', 'grape', "pineapple", "guave", "melon"]
let target = "grape"
let foundIndex = -1
for(let i = 0; i<fruits.length;i++){
    let currentNUmber=fruits[i]
    if(currentNUmber === target){
        foundIndex= i;
        console.log(foundIndex);
    }

}

if (foundIndex > -1){
    console.log(foundIndex,"found");
}
// -----------------------------------------------------------------------
// -----------------------------------------------------------------------
/// problems : 7.2 ///
/// Find array elements
let fruitss = ['mango', 'grape', "pineapple", "guave", "melon"]
let targets = "melon";
let foundIndexs = -1;

for ( let i = 0; i<fruitss.length ; i++){
    let currentNUmber= fruitss[i]
    if(currentNUmber === targets){
        foundIndex = i
    }
}

if (foundIndexs > -1){
    console.log(foundIndex,"found");
}/// output : 1 found // that means melon index number is 1 
// -----------------------------------------------------------------------

// -----------------------------------------------------------------------
/// problems : 7.3 ///
/// Find array elements
let fruit = ['mango', 'grape', "pineapple", "guave", "melon"]
let targe = "pink";
let foundInde = -1;
for ( let i = 0; i<fruit.length ; i++){
   let currentNUmber = fruit[i]
   if ( currentNUmber === targe){
        foundInde = i;
   }

}
if ( foundInde > -1){
    console.log(foundInde , found);
}else {
    console.log("the item is not found");
}

/// output : the item is not found // aejonnoi moloto foundeIndex -1 kora hoice , karon je nai tar index always -1
// -----------------------------------------------------------------------

// -----------------------------------------------------------------------
/// problems : 8 ///
/// Find Max/ Min number
let numb = [22,718,54]
let maxNumb = numb[0];
let minNumb = numb[0];

for (let i = 0; i<numb.length ; i++){
    let currentNumber = numb[i]
    if (maxNumb < currentNumber) {
        maxNumb = currentNumber // currentNumber er value e reset kore dicce 
        
    }
    if (minNumb > currentNumber) {
        minNumb = currentNumber // currentNumber er value e reset kore dicce 
        
    }
}
console.log(maxNumb,minNumb);

/// output : 718 22
// -----------------------------------------------------------------------

// -----------------------------------------------------------------------
/// problems : 9 ///
/// Filter an array
// using loop 
const purchase =[100, 200, 500, 300, 600]
const purchaseBOx = []

for (let i = 0; i<purchase.length ; i++){
    let currentElems = purchase[i];
    if( currentElems <= 200){
        purchaseBOx.push(currentElems)
    }
}
console.log(purchaseBOx);
/// output : [100, 200]
// -----------------------------------------------------------------------

// -----------------------------------------------------------------------
/// problems : 9.1///
/// Filter an array
// using .filter()
const purchases =[100, 200, 500, 300, 600]
for (let i = 0; i<purchases.length; i++){
    let currentElems = purchases[i]
}
const puchasebox = purchases.filter(function(currentElems){
return currentElems >= 200 // boolen true hole dokbe na hole ber hoe jabe
})

console.log(puchasebox);
/// output : [ 200, 500, 300, 600 ]
// -----------------------------------------------------------------------

// -----------------------------------------------------------------------
/// problems : 10///
/// calculating Discount 

const discountPrice = []
const purchases =[100, 200, 500, 300, 600]

for ( let i = 0; i<purchases.length ; i++){
    let currentElems = purchases[i]
    if ( currentElems > 200){
        // 10% discount 
        let discount = currentElems - (currentElems * 10/100);
        discountPrice.push(discount)
    }else {
        discountPrice.push(currentElems)
    }
}
console.log(discountPrice);
// -----------------------------------------------------------------------

// -----------------------------------------------------------------------
/// problems : 10.1///
/// calculating Discount 

const ShoppingPrice = [5000,1000,2000, 3000, 4000]
const discountPrice =[]

for (let i = 0; i<ShoppingPrice.length ; i++){
    let currentElems = ShoppingPrice[i]

    if ( currentElems > 2000){
        // 20% discount
        let discount = currentElems - currentElems * (20 /100)
        discountPrice.push(discount)
    }else {
        discountPrice.push(currentElems)
    }
}
console.log(discountPrice);

// -----------------------------------------------------------------------
// -----------------------------------------------------------------------
/// problems : 10.2///
/// calculating Discount 
/// using map method / foreach method

let shopping  = [500,240,1000, 5000, 7000]

// traversing Dont need any for loop when u are using map or filter
for ( let i= 0; i<shopping.length; i++){
    let currentElems = shopping[i]
}
// traversing

// using map
let shoppingUsingMap = shopping.map(function (currentElems) {
    if ( currentElems > 2000){
                // 20% discount
                let CalculatedPrice = currentElems - currentElems * (20 /100)
                return CalculatedPrice /// map use korle aar push kora lage na 
            }
            else { // without else result dibe : [ undefined, undefined, undefined, 4000, 5600 ]
                return currentElems
            }
})

console.log(shoppingUsingMap);
//output: [ 500, 240, 1000, 4000, 5600 ] , map er kaj protita elems ke modify kora ,protita

// -----------------------------------------------------------------------
// so whats the difference between map and filer ?
// map ekta array ke modify kore noton array te rupantor kore , sob element noton hoe jai.
// filter ekta array er upor condition calie jegula sorte tikbe sudo segulo ke nibe.

// ------------------------------------
// example map //
//map(): map() ek array ko traverse karta hai aur har element par ek function ko apply karta hai, fir ek naya array banata hai jismein har element ka modified version hota hai. Yeh modified version naye array mein store hota hai. Jaise ki:

let numbers = [1, 2, 3, 4, 5];

let doubledNumbers = numbers.map(function(num) {
    return num * 2;
});

console.log(doubledNumbers); // Output: [2, 4, 6, 8, 10]
// ------------------------------------
// ------------------------------------
// example filter //
//filter(): filter() ek array ko traverse karta hai aur ek condition ko check karta hai. Us condition ke base par, jo elements condition ko pass karte hain, woh naye array mein shamil hote hain. Jaise ki:

let numbers = [1, 2, 3, 4, 5];

let evenNumbers = numbers.filter(function(num) {
    return num % 2 === 0;
});

console.log(evenNumbers); // Output: [2, 4]

// ------------------------------------

// Toh sum up karte hue, map() ek array ke elements ko modify karke ek naya array banata hai, jabki filter() ek array ko filter karke ek naya array banata hai jo sirf certain conditions ko meet karte hain.
// -----------------------------------------------------------------------

// -----------------------------------------------------------------------
/// problems : 11 ///
/// Frequency array // kono sonka kotobar exist kore seta mone rakar array
/// using map method / foreach method

const Frequency = [0, 0, 0, 0, 0, 0, 0, 0, 0, 0]

const sampleNumber = '9223843002357834322' // ae sonka gulo doren akta index number 
// aekon check koren aekta index koto bar ase , se onojai tar index tar repitation bosbe

// Findout Maximum occurance
for (let i = 0; i <sampleNumber.length ; i++){
    let currentElems = sampleNumber[i]
    Frequency[currentElems]++
}
console.log(Frequency);


/// first of all , frequency namok aaray ase , jetar 10 ta item 0 nilam 
// varible declare korlam = '9223843002357834322';
//kaj ta kibabe korce ?
// first of all , i = 0 korce , condition dekce , current elems e dokse = sampleNumber[i] ,= 9 pacce , 
// sutorang currentElems er value holo 9 , 
// frequency[currentElems]++ aetar mane hole current elems 9 no index jabe , aemnite 9no index 0 ase,
// tar man jokon 9 no index dokbe tokon 1barbe, tar mane 9 ase ekbar 
[0, 0, 0, 0, 0, 0, 0, 0, 0, 1]
// sampleNumber = '9223843002357834322'
// thik tarpor i = 1 (1index) ; currentElems = sampleNumber[i] = currentElems = 2 hobe
// thik Frequency[currentElems]++ aeta te frequency[2]++ (2no index) er value(0) sate 1 jog hobe . 
[0, 0, 1, 0, 0, 0, 0, 0, 0, 1]
// aebabe barbe ...
// sobcea better use Debug & console.

// -----------------------------------------------------------------------
/// problems : 11 ///
//  Findout maximum occurance
frequency = [
  2, 0, 5, 5, 2,
  1, 0, 1, 2, 1
]
let maxOccurance = Frequency[0]; // dore nilam frequency aaray 1st onko ta 0 aetai maxOccurance
for ( let i =0 ; i<Frequency.length; i++){
    let currentElems = Frequency[i]

    if ( maxOccurance < currentElems){
            maxOccurance = currentElems
    }
}
console.log(maxOccurance);

// -----------------------------------------------------------------------

// -----------------------------------------------------------------------
/// problems : 11.1 ///
//  Findout maximum occurance & konsonka maximum bar asce
frequency = [
  2, 0, 5, 5, 2,
  1, 0, 1, 2, 1
]
let maxOccurance = Frequency[0]; // dore nilam frequency aaray 1st onko ta 0 aetai maxOccurance
let maxIndexNumber = 0
for ( let i =0 ; i<Frequency.length; i++){
    let currentElems = Frequency[i]

    if ( maxOccurance < currentElems){
            maxOccurance = currentElems
            maxIndexNumber = i;
    }
}
console.log(maxOccurance , maxIndexNumber,"is maximum repitation");

// -----------------------------------------------------------------------
/// problems : 11.2 ///
//  Findout maximum occurance & konsonka maximum bar asce

let frequency = [2, 6, 5, 5, 2,
    1, 7, 7, 2, 1]
let maxOccurance = frequency[0]
let maxIndexNumber = 0;

for ( let i = 0 ; i<frequency.length ;i++){
    let currentElems = frequency[i]

    if ( maxOccurance < currentElems){
        maxOccurance = currentElems;
        maxIndexNumber = i
    }
}

console.log(maxOccurance, maxIndexNumber);

// use debug & console to understand it .



       Know Most Advanced Loop and Array task <End>
=======================================================