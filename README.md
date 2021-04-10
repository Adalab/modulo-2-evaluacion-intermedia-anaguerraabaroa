![Random Number App](./images/app.png)

# **Random Number**

Half Module 2 project of the Adalab Digital Frontend Development Bootcamp.

This is an app to guess a random number developed with [<img src = "https://img.shields.io/badge/-HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white">](https://html.spec.whatwg.org/) [<img src="https://img.shields.io/badge/-SASS-cc6699?style=for-the-badge&logo=sass&logoColor=ffffff">](https://sass-lang.com/)
 [<img src = "https://img.shields.io/badge/-CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white">](https://www.w3.org/Style/CSS/) and [<img src="https://img.shields.io/badge/-SASS-cc6699?style=for-the-badge&logo=sass&logoColor=ffffff">](https://sass-lang.com/)

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

## **Listeners and functions**

### **Get random number**

- **Get initial random number:** function getRandomNumber(max)

### **Get user random number**

- **Event listener:** buttonElement.addEventListener("click", getFinalNumber)
- **Handle user random number and paint clues and attempts:** function getFinalNumber()

### **Get attempts to guess random number**

- **Handle attempts to guess random number:** function getAttemptsNumber()

## **Updating**

```
git add -A
git commit -m "Message commit"
git push
```

## **License**

This project is licensed under [**MIT License**](https://spdx.org/licenses/MIT.html).
