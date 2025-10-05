# 🖨️ clsPrint — C++ Utility Printing Class

A comprehensive and reusable **printing utility class** for C++ that helps you quickly output text, numbers, patterns, random data, mathematical results, and formatted console output.  
It integrates with helper classes like `clsString`, `clsMath`, and `clsUtil` to provide advanced functionality.

---
📁 Project Structure

📜 clsPrint.h — Core header file

📜 clsString.h — String helper (vowel check, etc.)

📜 clsMath.h — Math helper (prime, palindrome, perfect numbers, etc.)

📜 clsUtil.h — Utility (random char, keys, tabs, etc.)

📜 main.cpp — Testing file (example provided below)

📄 README.txt — Documentation file
---

## 🚀 Features Overview

| Category | Description |
|-----------|--------------|
| 🧾 Text Handling | Print strings, tabs, vowels, first letters, and words |
| 🔢 Numbers | Print digits, Fibonacci, even/odd/prime/palindrome/perfect numbers |
| 🎲 Random Generation | Generate random characters, upper/lower/special letters, and random keys |
| 🧮 Math Integration | Works with `clsMath` for various number property checks |
| 📅 Date & Time | Print day/month short names and formatted week headers |
| 💾 File Handling | Save strings directly to files |
| 🎮 Console Effects | Screen color change, sound alert, and game result screens |

---

## ⚙️ Example Usage (main.cpp)

#include <iostream>
#include "clsPrint.h"

using namespace std;

int main()
{
    // Example 1: Basic printing
    clsPrint::Print("Hello from clsPrint!\n");

    // Example 2: Print tabs
    cout << clsPrint::Tabs(3) << "Indented Text\n";

    // Example 3: Print numbers
    cout << "Prime numbers from 1 to 20: ";
    clsPrint::PrintPrimeNumbers(1, 20);

    cout << "Perfect numbers from 1 to 500: ";
    clsPrint::PrintPerfectNumbers(1, 500);

    // Example 4: Random character generation
    cout << "\nRandom upper letters: ";
    clsPrint::PrintRandomUpperLetters(5);

    // Example 5: String processing
    clsPrint::PrintFirstLetterOfWords("Hello World From clsPrint");
    clsPrint::PrintVowels("Programming is Fun!");

    // Example 6: Save to file
    clsPrint::SaveStringToFile("output.txt", "This is a saved line from clsPrint.");

    // Example 7: Display game results
    clsPrint::PrintGameResultsScreen();
    clsPrint::ShowGameOverScreen();

    // Example 8: Fibonacci example
    cout << "Fibonacci sequence (10 terms): ";
    clsPrint::PrintFibonatchiSerie(10);

    return 0;
}

---

## 🧪 Sample Output

Hello from clsPrint!
			Indented Text
Prime numbers from 1 to 20: 2 3 5 7 11 13 17 19
Perfect numbers from 1 to 500: 6 28 496

Random upper letters: KDJQT

 First Letter of this string 
H
W
F
C

 Vowels In String are : o a i i u

______________________________________________________
                   +++ Game Result +++
--------------------------------------------------------

                    + + + G a m e O v e r + + +
______________________________________________________

Fibonacci sequence (10 terms): 0 1 1 2 3 5 8 13 21 34

---

## 🧩 Class API Overview

| Function | Description |
|-----------|-------------|
| Print(string Text) | Print any text |
| Tabs(int count) | Return tab indentation string |
| PrintPrimeNumbers(int from, int to) | Print all primes in range |
| PrintEvenNumbers(int from, int to) | Print even numbers |
| PrintOddNumbers(int from, int to) | Print odd numbers |
| PrintPerfectNumbers(int from, int to) | Print perfect numbers |
| PrintPalindromeNums(int from, int to) | Print palindromic numbers |
| PrintFibonatchiSerie(int Number) | Print Fibonacci series |
| PrintFibonacciUsingRecurssion(short n, int prev1, int prev2) | Recursive Fibonacci |
| PrintFirstLetterOfWords(string) | Print first letters of words |
| PrintVowels(string) | Print vowels in a string |
| PrintEachWord(string) | Print each word separately |
| SaveStringToFile(string filename, string text) | Append string to file |
| DayShortName(short) | Return short day name (Sun, Mon, ...) |
