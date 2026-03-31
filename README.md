# javascript-2
checkpoint
// Reverse a String
const reverseString = (str) => str.split("").reverse().join("");

// Count Characters
const countCharacters = (str) => str.length;

// Capitalize Words
const capitalizeWords = (sentence) =>
  sentence
    .split(" ")
    .map(word => word.charAt(0).toUpperCase() + word.slice(1))
    .join(" ");

    // Find Maximum
const findMax = (arr) => Math.max(...arr);

// Find Minimum
const findMin = (arr) => Math.min(...arr);

// Sum of Array
const sumArray = (arr) =>
  arr.reduce((sum, num) => sum + num, 0);

// Filter Array (example: filter even numbers)
const filterArray = (arr, conditionFn) =>
  arr.filter(conditionFn);

  // Factorial
const factorial = (n) => {
  if (n < 0) return "Invalid number";
  let result = 1;
  for (let i = 1; i <= n; i++) {
    result *= i;
  }
  return result;
};

// Prime Number Check
const isPrime = (num) => {
  if (num <= 1) return false;
  for (let i = 2; i <= Math.sqrt(num); i++) {
    if (num % i === 0) return false;
  }
  return true;
};

// Fibonacci Sequence
const fibonacci = (n) => {
  let sequence = [0, 1];
  for (let i = 2; i < n; i++) {
    sequence.push(sequence[i - 1] + sequence[i - 2]);
  }
  return sequence.slice(0, n);
};
