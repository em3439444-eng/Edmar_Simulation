<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>EduQuiz Game</title>
<style>
  body {
    font-family: Arial, sans-serif;
    background: #f0f8ff;
    text-align: center;
    padding: 20px;
  }

  .container {
    background: white;
    padding: 20px;
    max-width: 500px;
    margin: auto;
    border-radius: 10px;
    box-shadow: 0 0 10px gray;
  }

  button {
    display: block;
    width: 100%;
    margin: 10px 0;
    padding: 10px;
    font-size: 16px;
    cursor: pointer;
  }

  #score {
    font-weight: bold;
    margin-top: 10px;
  }
</style>
</head>
<body>

<div class="container">
  <h2>📚 EduQuiz Game</h2>
  <p id="question">Loading question...</p>
  <div id="choices"></div>
  <p id="score">Score: 0</p>
</div>

<script>
const quiz = [
  {
    question: "What is the capital of the Philippines?",
    choices: ["Cebu", "Manila", "Davao", "Baguio"],
    answer: "Manila"
  },
  {
    question: "What is 5 + 3?",
    choices: ["5", "8", "10", "12"],
    answer: "8"
  },
  {
    question: "What planet do we live on?",
    choices: ["Mars", "Venus", "Earth", "Jupiter"],
    answer: "Earth"
  },
  {
    question: "What is the largest ocean on Earth?",
    choices: ["Atlantic", "Indian", "Pacific", "Arctic"],
    answer: "Pacific"
  },
  {
    question: "What is H2O commonly known as?",
    choices: ["Salt", "Water", "Oxygen", "Hydrogen"],
    answer: "Water"
  },
  {
    question: "How many days are in a week?",
    choices: ["5", "6", "7", "8"],
    answer: "7"
  },
  {
    question: "What is the square root of 16?",
    choices: ["2", "3", "4", "5"],
    answer: "4"
  },
  {
    question: "Who is the national hero of the Philippines?",
    choices: ["Bonifacio", "Rizal", "Aguinaldo", "Lapu-Lapu"],
    answer: "Rizal"
  },
  {
    question: "What is the boiling point of water?",
    choices: ["50°C", "100°C", "150°C", "200°C"],
    answer: "100°C"
  },
  {
    question: "What is the primary source of energy for Earth?",
    choices: ["Moon", "Sun", "Wind", "Water"],
    answer: "Sun"
  }
];

let current = 0;
let score = 0;

function loadQuestion() {
  if (current >= quiz.length) {
    document.querySelector(".container").innerHTML =
      `<h2>🎉 Game Over!</h2>
       <p>Your Score: ${score} / ${quiz.length}</p>
       <button onclick="location.reload()">Play Again</button>`;
    return;
  }

  let q = quiz[current];
  document.getElementById("question").innerText = q.question;

  let choicesDiv = document.getElementById("choices");
  choicesDiv.innerHTML = "";

  q.choices.forEach(choice => {
    let btn = document.createElement("button");
    btn.innerText = choice;
    btn.onclick = () => checkAnswer(choice);
    choicesDiv.appendChild(btn);
  });
}

function checkAnswer(choice) {
  if (choice === quiz[current].answer) {
    score++;
  }

  current++;
  document.getElementById("score").innerText = "Score: " + score;
  loadQuestion();
}

loadQuestion();
</script>

</body>
</html>
