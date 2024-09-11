# java--1

// run `node index.js` in the terminal

console.log(`Hello Node.js v${process.versions.node}!`);

var name = "홍길동"; // 이름 저장
let age = 25;        // 나이 저장
const location = "서울"; // 거주지 저장 


console.log(typeof name);    // "string"
console.log(typeof age);     // "number"
console.log(typeof location); // "string"


let num1 = 10; nn  
let num2 = 3;

console.log(num1 + num2); // 덧셈: 13
console.log(num1 - num2); // 뺄셈: 7
console.log(num1 * num2); // 곱셈: 30
console.log(num1 / num2); // 나눗셈: 3.33
console.log(num1 % num2); // 나머지: 1


let firstName = "길동";
let lastName = "홍";

let fullName = lastName + " " + firstName;
console.log(fullName); // "홍 길동"

let userAge = 17;

if (userAge >= 18) {
    console.log("성인입니다.");
} else {
    console.log("미성년자입니다.");
}

let status = (age >= 18) ? "성인" : "미성년자";
console.log(status); // "성인" 또는 "미성년자"

let day = 2; // 예: 1은 월요일, 2는 화요일 등

switch(day) {
    case 1:
        console.log("월요일");
        break;
    case 2:
        console.log("화요일");
        break;
    case 3:
        console.log("수요일");
        break;
    case 4:
        console.log("목요일");
        break;
    case 5:
        console.log("금요일");
        break;
    case 6:
        console.log("토요일");
        break;
    case 7:
        console.log("일요일");
        break;
    default:
        console.log("잘못된 요일");
}


for (let i = 1; i <= 10; i++) {
    console.log(i);
}

let i = 10;
while (i >= 1) {
    console.log(i);
    i--;
}


let fruits = ["사과", "바나나", "포도"];
fruits.push("오렌지"); // 배열 끝에 추가
fruits.shift(); // 첫 번째 과일 제거
console.log(fruits); // ["바나나", "포도", "오렌지"]


for (let fruit of fruits) {
    console.log(fruit);
}

let person = {
    name: "홍길동",
    age: 25,
    job: "개발자"
};

console.log(person.name); // "홍길동"
console.log(person.age);  // 25
console.log(person.job);  // "개발자"


person.address = "서울"; // 주소 속성 추가
person.job = "수석 개발자"; // 직업 속성 수정

console.log(person); // {name: "홍길동", age: 25, job: "수석 개발자", address: "서울"}

function addNumbers(num1, num2) {
    return num1 + num2;
}

console.log(addNumbers(5, 10)); // 15

const concatenateStrings = (str1, str2) => str1 + " " + str2;

console.log(concatenateStrings("안녕하세요", "세계")); // "안녕하세요 세계"


