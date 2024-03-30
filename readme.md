
=================================================

     Know Most Advanced Loop and Array task <Start>

=================================================
// problems <br>
<br>
- reverse an array <br>
- sum of array elements <br>
- swap array elements <br>
- Find Array elements <br>
- Find Max/ Min number <br>
- Filter an array <br>
- using .find() .filter() <br>
- calculating Discount <br>
- solving same problem using map/ foreach() <br>
- Frequency array <br>
- Findout maximum occurance <br>
- serial change<br>
<br>
// kono kaj ekadikbar korar jonno loop use hoi <br>
<br>
for ( let i = 0; i<5 ; i++){ <br>
    console.log(i)<br>
}<br>
// loop bebohar kore lav ki ?<br>
// amra jani array 1st index number 0 hoi , aaray size ja hoi tar last index 1 kom hoi<br>
<br>
<br>
// -----------------------------------------------------------------------<br>
/// problems: 1///<br>
/// forward loops with array<br>
// decl array , dec for loops<br>
// use log with arr name then [variable name (for)]<br>
<br>
let arr = ['mango', 'grape', "pineapple", "guave", "melon"] <br>
<br>
for (let i = 0; i<5 ; i++){<br>
    console.log(arr[i]);       // forward loop // i=0 index mango ke nise, i=1 index grape ke nise aebabe<br> choltese<br>
}<br>
// -----------------------------------------------------------------------<br>
/// problems : 2 ///<br>
/// Reversed loops with array<br>
// use decrement thats it .<br>
<br>
let arr = ['mango', 'grape', "pineapple", "guave", "melon"]<br>
<br>
for (let i = arr.length-1 ; i>=0 ; i--){<br>
    console.log(arr[i]);<br>
}<br>
// -----------------------------------------------------------------------<br>
<br>
/// problems : 3 ///<br>
/// sum of array element<br>
<br>
<br>
let number = [10, 20, 30, 40, 50, 60]<br>
let sum = 0<br>
// i = 0 means it stating from 0 index , i<number.length means i<6<br>
<br>
for(let i =0 ; i<number.length ; i++){ <br>
    const currentNUmber = number[i]<br>
    sum = sum + currentNUmber<br>
    console.log(sum);// ekdom ses sum i,e pura complete hole bosate cie , tiele console baire den<br>
    //console.log(currentNUmber);<br>
    //console.log(number[i]);<br>
}<br>
console.log(sum);<br>
// -----------------------------------------------------------------------
// -----------------------------------------------------------------------
<br>
/// problems : 4 ///<br>
/// substraction of array element<br>
<br>
<br>
let numbers = [10, 20, 30, 40, 50, 60]<br>
let substraction = 0<br>
// i = 0 means it stating from 0 index , i<number.length means i<6<br>
<br>
for ( let i = 0; i<numbers.length ; i++){<br>
    let currentNumbers = numbers[i]    // array theke number save kore seta variable e nicci e protibar<br>
    substraction = currentNumbers - substraction<br>
    //console.log(numbers[i]);<br>
}<br>
console.log(substraction);<br>
// -----------------------------------------------------------------------<br>
<br>
<br>
// -----------------------------------------------------------------------<br>
/// problems : 6 ///<br>
/// swap array elements<br>
 let numbers = [10, 20, 30, 40, 50, 60]<br>
// doren ami cie 1index 20 ; 3index 40 er jaigai jabe ; and 40 , 20 er jaigai jabe<br>
// -----------------------------------------------------------------------<br>
<br>
 let numbers = [10, 20, 30, 40, 50, 60]<br>
<br>
let temp = numbers[3]    // mone koren 40 harie jabe , taile save koren tare varible er modde<br>
numbers[3]= 20; /// 3index er value change korsi<br>
numbers[1]= temp // 1 index er value o change korsi , konta jeta ektu agge hariete niccilo<br>
console.log(numbers);<br>
-----------------------------------------------------------------------<br>
let numbers = [10, 20, 30, 40, 50, 60]<br>
<br>
let temp = numbers[5] // mone koren 60 harie jabe , taile save koren tare varible er modde<br>
numbers[5]= 10; /// 5index er value change korsi, jehoto 10 60er jaiga replace korbe<br>
numbers[0]= temp // 0 index er value o change korsi , konta jeta ektu agge hariete niccilo<br>
console.log(numbers);<br>
<br>
// -----------------------------------------------------------------------
/// problems : 7 ///<br>
/// Find array elements<br>
<br>
//let fruits = ['mango', 'grape', "pineapple", "guave", "melon"]<br>
//let target = "grape"<br>
//let foundIndex = -1<br>
for(let i = 0; i<fruits.length;i++){<br>
    let currentNUmber=fruits[i]<br>
<br>
    if(currentNUmber === target){<br>
        foundIndex= i;<br>
        console.log(foundIndex);<br>
    }<br>
<br>
}<br>

if (foundIndex > -1){<br>
    console.log(foundIndex,"found");<br>
}<br>
// -----------------------------------------------------------------------<br>
// -----------------------------------------------------------------------<br>
<br>
/// problems : 7.2 ///<br>
/// Find array elements<br>
<br>
let fruitss = ['mango', 'grape', "pineapple", "guave", "melon"]<br>
let targets = "melon";<br>
let foundIndexs = -1;<br>
<br>
for ( let i = 0; i<fruitss.length ; i++){<br>
    let currentNUmber= fruitss[i]<br>
<br>
    if(currentNUmber === targets){<br>
        foundIndex = i<br>
    }<br>
}<br>
<br>
if (foundIndexs > -1){<br>
    console.log(foundIndex,"found");<br>
}/// output : 1 found // that means melon index number is 1 <br>
// -----------------------------------------------------------------------<br>
<br>
// -----------------------------------------------------------------------
/// problems : 7.3 ///<br>
/// Find array elements<br>

let fruit = ['mango', 'grape', "pineapple", "guave", "melon"]<br>
let targe = "pink";<br>
let foundInde = -1;<br>
for ( let i = 0; i<fruit.length ; i++){<br>
   let currentNUmber = fruit[i]<br>
<br>
   if ( currentNUmber === targe){<br>
        foundInde = i;<br>
   }<br>
<br>
}<br>
if ( foundInde > -1){<br>
    console.log(foundInde , found);<br>
}else {<br>
    console.log("the item is not found");<br>
}<br>
<br>
/// output : the item is not found // aejonnoi moloto foundeIndex -1 kora hoice , karon je nai tar index always -1<br>
// -----------------------------------------------------------------------<br>
<br>
// -----------------------------------------------------------------------<br>
/// problems : 8 ///<br>
/// Find Max/ Min number<br>
<br>
let numb = [22,718,54]<br>
let maxNumb = numb[0];<br>
let minNumb = numb[0];<br>
<br>
for (let i = 0; i<numb.length ; i++){<br>
    let currentNumber = numb[i]<br>
<br>
    if (maxNumb < currentNumber) {<br>
        maxNumb = currentNumber // currentNumber er value e reset kore dicce <br>
        <br>
    }<br>
    if (minNumb > currentNumber) {<br>
        minNumb = currentNumber // currentNumber er value e reset kore dicce <br>
        <br>
    }<br>
}<br>
console.log(maxNumb,minNumb);<br>
<br>
/// output : 718 22<br>
// -----------------------------------------------------------------------<br>
<br>
// -----------------------------------------------------------------------<br>
<br>
<br>
/// problems : 9 ///<br>
/// Filter an array<br>
// using loop <br>

const purchase =[100, 200, 500, 300, 600]<br>
const purchaseBOx = []<br>
<br>
for (let i = 0; i<purchase.length ; i++){<br>
    let currentElems = purchase[i];<br>
<br>
    if( currentElems <= 200){<br>
        purchaseBOx.push(currentElems)<br>
    }<br>
}<br>
console.log(purchaseBOx);<br>
/// output : [100, 200]<br>
// -----------------------------------------------------------------------<br>
<br>
// -----------------------------------------------------------------------<br>
/// problems : 9.1///<br>
/// Filter an array<br>
// using .filter()<br>
<br>
const purchases =[100, 200, 500, 300, 600]<br>
<br>
<!-- for (let i = 0; i<purchases.length; i++){<br>
    let currentElems = purchases[i]<br>
} --> filter method use korle irretation er dorkar nai <br>
<br>
const puchasebox = purchases.filter(function(currentElems){<br>
return currentElems >= 200 // boolen true hole dokbe na hole ber hoe jabe<br>
})<br>
<br>
console.log(puchasebox);<br>
/// output : [ 200, 500, 300, 600 ]<br>
// -----------------------------------------------------------------------<br>
<br>
// -----------------------------------------------------------------------<br>
<br>
/// problems : 10///<br>
/// calculating Discount <br>
<br>
const discountPrice = []<br>
const purchases =[100, 200, 500, 300, 600]<br>
<br>
for ( let i = 0; i<purchases.length ; i++){ <br>
    let currentElems = purchases[i]<br>
<br>
    if ( currentElems > 200){<br>
        // 10% discount <br>
        let discount = currentElems - (currentElems * 10/100);<br>
        discountPrice.push(discount)<br>
    }else {<br>
        discountPrice.push(currentElems)<br>
    }<br>
}<br>
console.log(discountPrice);<br>
// -----------------------------------------------------------------------<br>
<br>
// -----------------------------------------------------------------------<br>
/// problems : 10.1///<br>
/// calculating Discount <br>
<br>
const ShoppingPrice = [5000,1000,2000, 3000, 4000]<br>
const discountPrice =[]<br>
<br>
for (let i = 0; i<ShoppingPrice.length ; i++){<br>
    let currentElems = ShoppingPrice[i]<br>
<br><br>
    if ( currentElems > 2000){<br>
        // 20% discount<br>
        let discount = currentElems - currentElems * (20 /100)<br>
        discountPrice.push(discount)<br>
    }else {<br>
        discountPrice.push(currentElems)<br>
    }<br>
}<br>
console.log(discountPrice);<br>
<br>
// -----------------------------------------------------------------------<br>
// -----------------------------------------------------------------------<br>
// -----------------------------------------------------------------------<br>
//<br>
/// problems : 10.2///<br>
/// calculating Discount <br>
/// using map method / foreach method<br>


<br>
<!-- // traversing Dont need any for loop when u are using map or filter<br>
for ( let i= 0; i<shopping.length; i++){<br>
    let currentElems = shopping[i]<br>
}<br>
// traversing --> iteration er kono dorkar nai , (filter(),map(),foreach())
<br>
// using map<br>
let shopping  = [500,240,1000, 5000, 7000]<br>
let shoppingUsingMap = shopping.map(function (currentElems) {<br>
    if ( currentElems > 2000){<br>
                // 20% discount<br>
                let CalculatedPrice = currentElems - currentElems * (20 /100)<br>
                return CalculatedPrice /// map use korle aar push kora lage na <br>
            }<br>
            else { // without else result dibe : [ undefined, undefined, undefined, 4000, 5600 ]<br>
                return currentElems<br>
            }<br>
})<br>
<br>
console.log(shoppingUsingMap);<br>
//output: [ 500, 240, 1000, 4000, 5600 ] , map er kaj protita elems ke modify kora ,protita<br>
<br>
// -----------------------------------------------------------------------<br>
// so whats the difference between map and filer ?<br>
// map ekta array ke modify kore noton array te rupantor kore , sob element noton hoe jai.<br>
// filter ekta array er upor condition calie jegula sorte tikbe sudo segulo ke nibe.<br>
<br>
// ------------------------------------<br>
// example map //<br>
//map(): map() ek array ko traverse karta hai aur har element par ek function ko apply karta hai, fir ek naya array banata <br>hai jismein har element ka modified version hota hai. Yeh modified version naye array mein store hota hai. Jaise ki:<br>
<br>
let numbers = [1, 2, 3, 4, 5];<br>

let doubledNumbers = numbers.map(function(num) {<br>
    return num * 2;<br>
});<br>
<br>
console.log(doubledNumbers); // Output: [2, 4, 6, 8, 10]<br>
// ------------------------------------<br>
// ------------------------------------<br>
// example filter //<br>
//filter(): filter() ek array ko traverse karta hai aur ek condition ko check karta hai. Us condition ke base par, jo<br> elements condition ko pass karte hain, woh naye array mein shamil hote hain. Jaise ki:<br>
<br>
let numbers = [1, 2, 3, 4, 5];<br>
<br>
let evenNumbers = numbers.filter(function(num) { <br>
    return num % 2 === 0; <br>
}); <br>
<br>
console.log(evenNumbers); // Output: [2, 4]<br>
<br>
// ------------------------------------<br>
<br>
// Toh sum up karte hue, map() ek array ke elements ko modify karke ek naya array banata hai, jabki filter() ek array ko <br> filter karke ek naya array banata hai jo sirf certain conditions ko meet karte hain.<br>
// -----------------------------------------------------------------------<br>
<br>
// -----------------------------------------------------------------------<br>
/// problems : 11 ///<br>
/// Frequency array // kono sonka kotobar exist kore seta mone rakar array<br>
/// using map method / foreach method<br>
<br>
const Frequency = [0, 0, 0, 0, 0, 0, 0, 0, 0, 0]<br>
<br>
const sampleNumber = '9223843002357834322' // ae sonka gulo doren akta index number <br>
// aekon check koren aekta index koto bar ase , se onojai tar index tar repitation bosbe <br>
<br>
// Findout Maximum occurance<br>
<br>
const Frequency = [0, 0, 0, 0, 0, 0, 0, 0, 0, 0]<br>
const sampleNumber = '9223843002357834322'<br>
for (let i = 0; i <sampleNumber.length ; i++){<br>
    let currentElems = sampleNumber[i]<br>
    Frequency[currentElems]++ // as a example 9 no index er value (0) er sate 1 jog tokon 1bar frequency <br>
}<br>
console.log(Frequency);<br>
<br>
<br>
/// first of all , frequency namok aaray ase , jetar 10 ta item 0 nilam <br>
// varible declare korlam = '9223843002357834322';<br>
//kaj ta kibabe korce ?<br>
// first of all , i = 0 korce , condition dekce , current elems e dokse = sampleNumber[i] ,= 9 pacce , <br>
// sutorang currentElems er value holo 9 , <br>
// frequency[currentElems]++ aetar mane hole current elems 9 no index jabe , aemnite 9no index 0 ase,<br>
// tar man jokon 9 no index dokbe tokon 1barbe, tar mane 9 ase ekbar <br>
[0, 0, 0, 0, 0, 0, 0, 0, 0, 1]<br>
// sampleNumber = '9223843002357834322'<br>
// thik tarpor i = 1 (1index) ; currentElems = sampleNumber[i] = currentElems = 2 hobe<br>
// thik Frequency[currentElems]++ aeta te frequency[2]++ (2no index) er value(0) sate 1 jog hobe . <br>
[0, 0, 1, 0, 0, 0, 0, 0, 0, 1]<br>
// aebabe barbe ...<br>
// sobcea better use Debug & console.<br>
<br>
// -----------------------------------------------------------------------<br>
<br>
/// problems : 11 ///<br>
//  Findout maximum occurance<br>
frequency = [<br>
  2, 0, 5, 5, 2,<br>
  1, 0, 1, 2, 1<br>
]<br>
let maxOccurance = Frequency[0]; // dore nilam frequency aaray 1st onko ta 0 aetai maxOccurance<br>
for ( let i =0 ; i<Frequency.length; i++){<br>
    let currentElems = Frequency[i]<br>
<br>
    if ( maxOccurance < currentElems){<br>
            maxOccurance = currentElems<br>
    }<br>
}<br>
console.log(maxOccurance);<br>
<br>
// -----------------------------------------------------------------------<br>
<br>
// -----------------------------------------------------------------------<br>
/// problems : 11.1 ///<br>
//  Findout maximum occurance & konsonka maximum bar asce<br>
frequency = [ <br>
  2, 0, 5, 5, 2,<br>
  1, 0, 1, 2, 1<br>
]<br>
let maxOccurance = Frequency[0]; // dore nilam frequency aaray 1st onko ta 0 aetai maxOccurance<br>
let maxIndexNumber = 0<br>
for ( let i =0 ; i<Frequency.length; i++){<br>
    let currentElems = Frequency[i] <br>
<br>
    if ( maxOccurance < currentElems){<br>
            maxOccurance = currentElems<br>
            maxIndexNumber = i;<br>
    }<br>
}<br>
console.log(maxOccurance , maxIndexNumber,"is maximum repitation");<br>
<br>
// -----------------------------------------------------------------------<br>
/// problems : 11.2 ///<br>
//  Findout maximum occurance & konsonka maximum bar asce<br>
<br>
let frequency = [2, 6, 5, 5, 2,<br>
    1, 7, 7, 2, 1]<br>
let maxOccurance = frequency[0]<br>
let maxIndexNumber = 0;<br>
<br>
for ( let i = 0 ; i<frequency.length ;i++){<br>
    let currentElems = frequency[i]<br>
<br>
    if ( maxOccurance < currentElems){<br>
        maxOccurance = currentElems;<br>
        maxIndexNumber = i<br>
    } <br>
}<br>
<br>
console.log(maxOccurance, maxIndexNumber);<br>
<br>
// use debug & console to understand it .<br>



       Know Most Advanced Loop and Array task <End>
=======================================================