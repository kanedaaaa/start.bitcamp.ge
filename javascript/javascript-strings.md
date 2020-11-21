**სტრინგები**

ჯავასკრიპტში სტრინგები უნიკოდირებული სიმბოლოებია (Unicode characters), რაც კარგი ამბავია იმ ადამიანებისთვის
ვისაც ინტერნაციონალურ პროექტებზე უწევს მუშაობა. უფრო კონკრეტულად, სტრინგები UTF-16 კოდის დანაყოფებია.
თითოეული დანაყოფი არის 16 ბიტიანი რიცხვით წარმოდგენილი. სტანდარტულად სიმბოლოები ერთი, ან ორი
დანაყოფით არის წარმოდგენილი.

სტრინგის (ზემოთ ნახსენები კოდის დანაყოფები) სიგრძის გასაგებად შეგვიძლია ```length``` საკუთრების გამოყენება:

```
'hello'.length; // 5
```
უკვე ვთქვი რომ სტრინგები ობიექტებივითაა? მათ აქვს მეთოდები, რაც სტრინგებით მანიპულირების საშუალებას გაძლევს:

```
'hello'.charAt(0); // "h"
'hello', world'.replace('world', 'mars'); // "hello, mars"
'hello'.toUpperCase(); // "HELLO"
```