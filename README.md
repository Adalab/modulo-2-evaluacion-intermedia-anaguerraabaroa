![Random Number App](./images/app.png)

# **Random Number**

Half Module 2 project of the Adalab Digital Frontend Development Bootcamp.

This is an app to guess a random number developed with [<img src = "https://img.shields.io/badge/-HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white">](https://html.spec.whatwg.org/) [<img src="https://img.shields.io/badge/-SASS-cc6699?style=for-the-badge&logo=sass&logoColor=ffffff">](https://sass-lang.com/)
[<img src = "https://img.shields.io/badge/-CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white">](https://www.w3.org/Style/CSS/) and [<img src = "https://img.shields.io/badge/-JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">](https://www.ecma-international.org/ecma-262/)

## **Quick start guide**

Instructions to start this project:

### Installation

- Clone repository:

```
git clone [repository]
```

- Run project on local server with VSCode live server plugin.

- **[Project URL](https://anaguerraabaroa.github.io/random-number/)** is also available on GitHub Pages.

## **Project features**

- Generate a random number with methods Math.random and Math.ceil when app runs
- Input to enter a random number manually
- Button to send manual random number to app
- Inputs for clues and attemps to guess random number. Clues help user to find if manual random number matchs with generated random number

## **Usage**

### **Get random number**

```javascript
function getRandomNumber(max) {
  return Math.ceil(Math.random() * max);
}
```

### **App handler**

```javascript
function getFinalNumber() {
  const userNumber = parseInt(inputElement.value);
  console.log(userNumber);
  if (userNumber > 0 && userNumber <= 100) {
    if (userNumber > randomNumber) {
      clueElement.innerHTML = "Pista: demasiado alto";
    } else if (userNumber < randomNumber) {
      clueElement.innerHTML = "Pista: demasiado bajo";
    } else if (userNumber === randomNumber) {
      clueElement.innerHTML = "Has ganado campeona!!!";
    }
  } else {
    clueElement.innerHTML = "Pista: el número debe estar entre 1 y 100";
  }
  attemptsElement.innerHTML = getAttemptsNumber();
}
```

### **Get attempts to guess number**

```javascript
function getAttemptsNumber() {
  attempts++;
  return `Número de intentos: ${attempts}`;
}
```

## **Folder Structure**

```
Random Number
├── images
│   └── app.png
├── styles
│   └── main.css
├── index.html
├── LICENSE
├── main.js
└── README.md
```

## **License**

This project is licensed under ![GitHub](https://img.shields.io/github/license/anaguerraabaroa/random-number?label=License&logo=MIT&style=for-the-badge)
