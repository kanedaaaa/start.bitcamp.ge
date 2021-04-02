**საკონტროლო სტრუქტურები**

როგორც სხვა მრავალ პროგრამირების ენაში, ჯავაკსრიპტსაც გააჩნია კონდიციური სთეითმენთები
`if`, `else` და `else if`. მათი გადაბმით კი მიიღება საინტერესო სტრუქტურები:

```javascript
var name = 'kittens';
if (name === 'puppies') {
  name += ' woof';
} else if (name === 'kittens') {
  name += ' meow';
} else {
  name += '!';
}
name === 'kittens meow';
```
ასევე, ჯავასკრიპტში შეხვდებით `while` და `do-while` მარყუჟებს.

```javascript
while (true) {
  // სამუდამო მარყუჟი
}

var input;
do {
  input = get_input();
} while (inputIsNotValid(input)); 
```
`for` მარყუჟიც აქვეა:

```javascript
for (var i = 0; i < 5; i++) {
  // მარყუჟის სხეული გაეშვება ხუთჯერ 
}
```javascript
`for...of` და `for...in` მარყუჟები, მეტად კონკრეტული შემთხვევისთვის:

```javascript
for (let value of array) // ან let property in object
```
ზემოთ მოცემულ მარყუჟებში აქტუალურია ლოგიკური ოპერატორების გამოყენება (და არამარტო)
`&&` - და, `||` - ან.

ასევე ოდნავ უცნაური ternary ოპერატორი რომელიც if-else სთეითმენთის შემოკლებული ვარიანტია:

```javascript
var allowed = (age>18) ? 'yes' : 'no'
```
და sweet old switch სთეითმენთი რომელსაც ასევე if-else ფუნქციას ასრულებს, მაგრამ 
წასაკითხად მეტად სასიამოვნოა:

```javascript
switch (action) {
  case 'draw':
    drawIt();
    break;
  case 'eat':
    eatIt();
    break;
  default:
    doNothing();
}
```

იმ შემთხვევაში თუ break_ს არ გამოიყენებთ, მთელი სთეითმენთი "ჩაიქცევა", რაც გამიზნულად 
არ გენდომებათ. თუ მსგავს ქმედებას გამიზნულად აკეთებთ, კარგი იქნება თუ კომენტარსაც დაურთავთ:

```javascript
switch (a) {
  case 1: // fallthrough
  case 2:
    eatIt();
    break;
  default:
    doNothing();
}
```

