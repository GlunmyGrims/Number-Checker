# Number Checker

![MIT License](https://img.shields.io/badge/MIT-green?style=for-the-badge) 
![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E)
[![roadmap.sh](https://img.shields.io/badge/roadmap.sh-Project%20Idea-blue?style=for-the-badge&logo=roadmapdotsh)](https://roadmap.sh/projects/js-number-checker)

A lightweight, flexible, and dependency-free vanilla JavaScript utility library designed to quickly analyze and validate numbers. Perfect for form validation, lightweight math tests, simple CAPTCHAs, debugging, and testing.

---

## Features

- **Instant Analysis:** Quickly retrieve a comprehensive set of characteristics for any given number.
- **Modular Architecture:** Every function has a single responsibility, allowing you to import or copy only what your project needs.
- **Lightweight & Fast:** Built entirely in vanilla JavaScript with zero external dependencies.
- **Developer-Friendly:** Designed to make debugging and input validation effortless.

## Technologies Used

- **JavaScript (Vanilla):** Chosen for its simplicity, flexibility, zero-overhead performance, and universal compatibility in web development.

## Challenges Faced

Implementing the even and odd checks efficiently proved slightly tricky when trying to rely on a single core function. However, by leveraging the logical NOT (`!`) operator in combination with the even check, the solution became clean, concise, and performant.

## How to Use

1. Clone or download the source code into your project directory.
2. Import the functions into your module or simply copy and paste the utilities you need.

### Example Usage

```javascript
function describeNumber(number) {
    let output = {
        positive: isPositive(number),
        negative: isNegative(number),
        zero: isZero(number),
        even: isEven(number),
        odd: !isEven(number)
    };

    return output;
}

console.log(describeNumber(8));

/* Output:
{ 
    positive: true, 
    negative: false, 
    zero: false, 
    even: true, 
    odd: false 
}
*/
```

## License

This project is licensed under the MIT License.

## Links & Resources

- **Roadmap Project Specification:** [JavaScript Number Checker](https://roadmap.sh/projects/js-number-checker)
# Number-Checker
