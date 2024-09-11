# java--1

// run `node index.js` in the terminal

console.log(`Hello Node.js v${process.versions.node}!`);
// 1. 변수 선언과 할당
var name = "홍길동"; // 이름 저장
let age = 25;        // 나이 저장
const location = "서울"; // 거주지 저장 

// 2. 데이터 타입 확인
console.log(typeof name);    // "string"
console.log(typeof age);     // "number"
console.log(typeof location); // "string"

// 3. 산술 연산
let num1 = 10; nn  
let num2 = 3;

console.log(num1 + num2); // 덧셈: 13
console.log(num1 - num2); // 뺄셈: 7
console.log(num1 * num2); // 곱셈: 30
console.log(num1 / num2); // 나눗셈: 3.33
console.log(num1 % num2); // 나머지: 1

// 4. 문자열 연결
let firstName = "길동";
let lastName = "홍";

let fullName = lastName + " " + firstName;
console.log(fullName); // "홍 길동"

// 5. 조건문
let userAge = 17;

if (userAge >= 18) {
    console.log("성인입니다.");
} else {
    console.log("미성년자입니다.");
}

// 6. 삼항 연산자
let status = (age >= 18) ? "성인" : "미성년자";
console.log(status); // "성인" 또는 "미성년자"

// 7. switch문
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

// 8. for 반복문
for (let i = 1; i <= 10; i++) {
    console.log(i);
}

// 9. while 반복문
let i = 10;
while (i >= 1) {
    console.log(i);
    i--;
}

// 10. 배열 조작
let fruits = ["사과", "바나나", "포도"];
fruits.push("오렌지"); // 배열 끝에 추가
fruits.shift(); // 첫 번째 과일 제거
console.log(fruits); // ["바나나", "포도", "오렌지"]

// 11. 배열 순회
for (let fruit of fruits) {
    console.log(fruit);
}

// 12. 객체 생성
let person = {
    name: "홍길동",
    age: 25,
    job: "개발자"
};

console.log(person.name); // "홍길동"
console.log(person.age);  // 25
console.log(person.job);  // "개발자"

// 13. 객체 속성 추가/수정
person.address = "서울"; // 주소 속성 추가
person.job = "수석 개발자"; // 직업 속성 수정

console.log(person); // {name: "홍길동", age: 25, job: "수석 개발자", address: "서울"}

// 14. 함수 정의
function addNumbers(num1, num2) {
    return num1 + num2;
}

console.log(addNumbers(5, 10)); // 15

// 15. 화살표 함수
const concatenateStrings = (str1, str2) => str1 + " " + str2;

console.log(concatenateStrings("안녕하세요", "세계")); // "안녕하세요 세계"

// 16. 함수에서 객체 반환
function createPerson(name, age) {
    return {
        name: name,
        age: age
    };
}

let newPerson = createPerson("김철수", 30);
console.log(newPerson); // {name: "김철수", age: 30}

// 17. 클래스 정의
class Person {
    constructor(name, age) {
        this.name = name;
        this.age = age;
    }
}

let person1 = new Person("이영희", 22);
console.log(person1.name); // "이영희"
console.log(person1.age);  // 22

// 18. 클래스 상속
class Employee extends Person {
    constructor(name, age, job) {
        super(name, age);
        this.job = job;
    }
}

let employee1 = new Employee("박민수", 29, "디자이너");
console.log(employee1.name); // "박민수"
console.log(employee1.age);  // 29
console.log(employee1.job);  // "디자이너"

// 19. 객체의 메서드
class PersonWithGreet {
    constructor(name, age) {
        this.name = name;
        this.age = age;
    }

    greet() {
        console.log(`안녕하세요, 저는 ${this.name}입니다.`);
    }
}

let person2 = new PersonWithGreet("이영희", 22);
person2.greet(); // "안녕하세요, 저는 이영희입니다."

// 20. 배열 메서드
let numbers = [1, 2, 3, 4, 5];

let multipliedNumbers = numbers.map(num => num * 2);
console.log(multipliedNumbers); // [2, 4, 6, 8, 10]
