# 🧮 Math Quiz — C++

A console-based Math Quiz game built in **C++** demonstrating
core concepts of **Functional & Procedural Programming**.

---

## 🎯 Learning Objectives

- Structuring a program using functions (Procedural Programming)
- Separating logic, data, and display layers
- Using `enum` and `struct` as data models
- Passing data between functions cleanly
- Random number generation with `rand()` and `srand()`

---

## 🕹️ How to Play

1. Run the program
2. Choose how many questions (1–10)
3. Choose difficulty level:
   - `1` = Easy (1–10)
   - `2` = Med (10–50)
   - `3` = Hard (50–100)
   - `4` = Mix
4. Choose operation type:
   - `1` = Add
   - `2` = Sub
   - `3` = Mul
   - `4` = Div
   - `5` = Mix
5. Answer each question correctly to PASS!

> 🟢 Screen turns **green** for correct answer  
> 🔴 Screen turns **red** for wrong answer

---

## 🏗️ Project Architecture

```
main()
 └── StartGame()
      └── PlayMathGame()
           ├── ReadHowManyQuestions()
           ├── ReadQuestionsLevel()
           ├── ReadOpType()
           ├── GenerateQuizzQuestions()
           │    └── GenerateQuestion()
           │         └── SimpleCalculator()
           ├── AskAndCorrectQuestionListAnswers()
           │    ├── PrintTheQuestion()
           │    ├── ReadQuestionAnswer()
           │    └── CorrectTheQuestionAnswer()
           │         └── SetScreenColor()
           └── PrintQuizzResults()
```

---

## 💡 Key Concepts

| Concept                  | Where in Code                               |
| ------------------------ | ------------------------------------------- |
| Enums as named constants | `enQuestionsLevel`, `enOperationType`       |
| Structs as data models   | `stQuestion`, `stQuizz`                     |
| Pure logic functions     | `SimpleCalculator()`, `GenerateQuestion()`  |
| Display functions        | `PrintTheQuestion()`, `PrintQuizzResults()` |
| Game loop                | `StartGame()`, `PlayMathGame()`             |

---

## 🔧 Build & Run

**Open in Visual Studio**

```
double click: math-quiz-cpp.slnx
Ctrl + F5
```

**Windows (MinGW / g++)**

```bash
g++ math-quiz-cpp.cpp -o quiz.exe
./quiz.exe
```

---

## 📁 File Structure

```
math-quiz-cpp/
├── .gitignore
├── README.md
├── LICENSE
├── math-quiz-cpp.slnx
└── math-quiz-cpp/
    ├── math-quiz-cpp.cpp
    ├── math-quiz-cpp.vcxproj
    └── math-quiz-cpp.vcxproj.filters
```

---

## 👤 Author

Built as a learning exercise in C++ Procedural Programming.

---

## 📄 License

MIT License
