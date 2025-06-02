# 📅 Day 1 - Learn the Basics & Sorting Techniques

## ✅ Question 1: Fibonacci Number
- 🔗 Problem: [LeetCode - Fibonacci Number](https://leetcode.com/problems/fibonacci-number/)
- 📹 Tutorial: [Take U Forward](https://takeuforward.org/arrays/print-fibonacci-series-up-to-nth-term/)

```cpp
int fib(int n) {
    if(n == 0) return 0;
    if(n == 1) return 1;
    return fib(n - 1) + fib(n - 2);
}
// Time Complexity: O(2^n)
// Space Complexity: O(n) due to recursion stack
```

---

## ✅ Question 2: GCD or HCF of Two Numbers
- 🔗 Problem: [GFG - GCD of Two Numbers](https://www.geeksforgeeks.org/problems/gcd-of-two-numbers3459/1)
- 📹 Tutorial: [Take U Forward](https://takeuforward.org/data-structure/find-gcd-of-two-numbers/)

### 🔹 Solution 1: Brute Force (Ascending Loop)
```cpp
int gcd(int a, int b) {
    int ans = 1;
    int n = min(a, b);
    for(int i = 1; i <= n; i++) {
        if(a % i == 0 && b % i == 0) {
            ans = i;
        }
    }
    return ans;
}
// Time Complexity: O(min(a, b))
// Space Complexity: O(1)
```

---

### 🔹 Solution 2: Brute Force (Descending Loop)
```cpp
int gcd(int a, int b) {
    int n = min(a, b);
    for(int i = n; i >= 0; i--) {
        if(a % i == 0 && b % i == 0) {
            return i;
        }
    }
    return 1;
}
// Time Complexity: O(min(a, b))
// Space Complexity: O(1)
```

---

### 🔹 Solution 3: Recursive Subtraction Method
```cpp
int gcd(int a, int b) {
    if(a == 0 || b == 0) {
        return max(a, b);
    }
    int x = max(a, b);
    int y = min(a, b);
    return gcd(x - y, y);
}
// Time Complexity: O(max(a, b)) in worst case
// Space Complexity: O(max(a, b)) due to recursion
```

---

### 🔹 Solution 4: Euclidean Algorithm (Efficient)
```cpp
int gcd(int a, int b) {
    return b ? gcd(b, a % b) : a;
}
// Time Complexity: O(log(min(a, b)))
// Space Complexity: O(log(min(a, b))) due to recursion
```

---

## ✅ Question 3: Sum of First N Numbers
- 📹 Tutorial: [Take U Forward](https://takeuforward.org/data-structure/sum-of-first-n-natural-numbers/)

```cpp
void solve(int N) {
    int sum = N * (N + 1) / 2;
    cout<<"The sum of the first "<<N<<" numbers is: "<<sum<<endl;
  }

// Time Complexity: O(1)
// Space Complexity: O(1)
```

---

## ✅ Question 4: Bubble Sort
- 📹 Tutorial: [Take U Forward](https://takeuforward.org/data-structure/bubble-sort-algorithm/)

```cpp
// Add your Bubble Sort solution here when ready
```

---

## ✅ Question 5: Recursive Insertion Sort
- 📹 Tutorial: [Take U Forward](https://takeuforward.org/arrays/recursive-insertion-sort-algorithm/)

```cpp
// Add your Recursive Insertion Sort solution here when ready
```

---

## ✅ Question 6: Selection Sort
- 📹 Tutorial: [Take U Forward](https://takeuforward.org/sorting/selection-sort-algorithm/)

```cpp
// Add your Selection Sort solution here when ready
```

---

## ✅ Question 7: Majority Element (> n/2 times)
- 🔗 Problem: [LeetCode - Majority Element](https://leetcode.com/problems/majority-element/)
- 📹 Tutorial: [Take U Forward](https://takeuforward.org/data-structure/find-the-majority-element-that-occurs-more-than-n-2-times/)

```cpp
// Add your Majority Element solution here when ready
```
