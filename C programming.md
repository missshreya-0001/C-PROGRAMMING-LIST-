# C-PROGRAMMING-LIST-
# List of Basic C Programs

A collection of beginner-friendly C programming examples. Each program includes the code and sample output.

---

## 1. Hello World

```c
#include <stdio.h>

int main() {
    printf("Hello, World!\n");
    return 0;
}
```
**Output:**
```
Hello, World!
```

---

## 2. Arithmetic Operations (Predefined Values)

```c
#include <stdio.h>

int main() {
    int a = 10, b = 5;
    printf("Sum = %d\n", a + b);
    printf("Difference = %d\n", a - b);
    printf("Product = %d\n", a * b);
    printf("Quotient = %d\n", a / b);
    return 0;
}
```
**Output:**
```
Sum = 15
Difference = 5
Product = 50
Quotient = 2
```

---

## 3. Arithmetic Operations (Input from User)

```c
#include <stdio.h>

int main() {
    int a, b;
    printf("Enter two numbers: ");
    scanf("%d %d", &a, &b);
    printf("Sum = %d\n", a + b);
    printf("Difference = %d\n", a - b);
    printf("Product = %d\n", a * b);
    printf("Quotient = %d\n", a / b);
    return 0;
}
```
**Output (Example):**
```
Enter two numbers: 8 4
Sum = 12
Difference = 4
Product = 32
Quotient = 2
```

---

## 4. Swap of Two Variables Using Third Variable

```c
#include <stdio.h>

int main() {
    int a = 5, b = 10, temp;
    temp = a;
    a = b;
    b = temp;
    printf("a = %d, b = %d\n", a, b);
    return 0;
}
```
**Output:**
```
a = 10, b = 5
```

---

## 5. Swap of Two Variables Without Using Third Variable

```c
#include <stdio.h>

int main() {
    int a = 5, b = 10;
    a = a + b;
    b = a - b;
    a = a - b;
    printf("a = %d, b = %d\n", a, b);
    return 0;
}
```
**Output:**
```
a = 10, b = 5
```

---

## 6. Area and Perimeter of Rectangle

```c
#include <stdio.h>

int main() {
    float length = 5.0, width = 3.0;
    printf("Area = %.2f\n", length * width);
    printf("Perimeter = %.2f\n", 2 * (length + width));
    return 0;
}
```
**Output:**
```
Area = 15.00
Perimeter = 16.00
```

---

## 7. Simple Interest

```c
#include <stdio.h>

int main() {
    float p = 1000, r = 5, t = 2;
    float si = (p * r * t) / 100;
    printf("Simple Interest = %.2f\n", si);
    return 0;
}
```
**Output:**
```
Simple Interest = 100.00
```

---

## 8. Celsius to Fahrenheit and Fahrenheit to Celsius

```c
#include <stdio.h>

int main() {
    float c = 37, f;
    f = (c * 9/5) + 32;
    printf("%.2f Celsius = %.2f Fahrenheit\n", c, f);

    f = 98.6;
    c = (f - 32) * 5/9;
    printf("%.2f Fahrenheit = %.2f Celsius\n", f, c);
    return 0;
}
```
**Output:**
```
37.00 Celsius = 98.60 Fahrenheit
98.60 Fahrenheit = 37.00 Celsius
```

---

## 9. Convert Days into Years, Weeks, Days

```c
#include <stdio.h>

int main() {
    int days = 375, years, weeks;
    years = days / 365;
    weeks = (days % 365) / 7;
    days = days - (years * 365) - (weeks * 7);
    printf("%d Years, %d Weeks, %d Days\n", years, weeks, days);
    return 0;
}
```
**Output:**
```
1 Years, 1 Weeks, 3 Days
```

---

## 10. Volume of Sphere

```c
#include <stdio.h>
#define PI 3.14159

int main() {
    float radius = 3.0;
    float volume = (4.0/3) * PI * radius * radius * radius;
    printf("Volume = %.2f\n", volume);
    return 0;
}
```
**Output:**
```
Volume = 113.10
```

---

## 11. Convert Minutes to Hours and Minutes

```c
#include <stdio.h>

int main() {
    int minutes = 135;
    int hrs = minutes / 60;
    int mins = minutes % 60;
    printf("%d Hours, %d Minutes\n", hrs, mins);
    return 0;
}
```
**Output:**
```
2 Hours, 15 Minutes
```

---

## 12. Collinear Points Check

```c
#include <stdio.h>

int main() {
    int x1=1, y1=2, x2=2, y2=4, x3=3, y3=6;
    if ((y2-y1)*(x3-x2) == (y3-y2)*(x2-x1))
        printf("Points are collinear\n");
    else
        printf("Points are not collinear\n");
    return 0;
}
```
**Output:**
```
Points are collinear
```

---

## 13. Largest Among Three Numbers

```c
#include <stdio.h>

int main() {
    int a=10, b=25, c=15;
    if(a >= b && a >= c)
        printf("Largest = %d\n", a);
    else if(b >= a && b >= c)
        printf("Largest = %d\n", b);
    else
        printf("Largest = %d\n", c);
    return 0;
}
```
**Output:**
```
Largest = 25
```

---

## 14. Largest of Two Numbers

```c
#include <stdio.h>

int main() {
    int a=10, b=25;
    if(a > b)
        printf("%d is larger\n", a);
    else
        printf("%d is larger\n", b);
    return 0;
}
```
**Output:**
```
25 is larger
```

---

## 15. Check if Number is Positive, Negative, or Zero

```c
#include <stdio.h>

int main() {
    int num = -5;
    if(num > 0)
        printf("Positive\n");
    else if(num < 0)
        printf("Negative\n");
    else
        printf("Zero\n");
    return 0;
}
```
**Output:**
```
Negative
```

---

## 16. Even or Odd

```c
#include <stdio.h>

int main() {
    int num = 6;
    if(num % 2 == 0)
        printf("Even\n");
    else
        printf("Odd\n");
    return 0;
}
```
**Output:**
```
Even
```

---

## 17. Gross Salary Calculation

```c
#include <stdio.h>

int main() {
    float basic = 20000, da, hra, gross;
    da = 0.8 * basic;
    hra = 0.1 * basic;
    gross = basic + da + hra;
    printf("Gross Salary = %.2f\n", gross);
    return 0;
}
```
**Output:**
```
Gross Salary = 38000.00
```

---

## 18. Division of Student on 5 Subjects

```c
#include <stdio.h>

int main() {
    int m1=70, m2=65, m3=80, m4=75, m5=60;
    float avg = (m1 + m2 + m3 + m4 + m5) / 5.0;
    if(avg >= 60)
        printf("First Division\n");
    else if(avg >= 45)
        printf("Second Division\n");
    else if(avg >= 33)
        printf("Third Division\n");
    else
        printf("Fail\n");
    return 0;
}
```
**Output:**
```
First Division
```

---

## 19. Discount on Purchasing Items

```c
#include <stdio.h>

int main() {
    float price = 1200, discount, final;
    if(price > 1000)
        discount = price * 0.10;
    else
        discount = price * 0.05;
    final = price - discount;
    printf("Final Price = %.2f\n", final);
    return 0;
}
```
**Output:**
```
Final Price = 1080.00
```

---

## 20. Check Character: Alphabet, Digit, or Special Character

```c
#include <stdio.h>

int main() {
    char ch = '*';
    if ((ch >= 'A' && ch <= 'Z') || (ch >= 'a' && ch <= 'z'))
        printf("Alphabet\n");
    else if (ch >= '0' && ch <= '9')
        printf("Digit\n");
    else
        printf("Special Character\n");
    return 0;
}
```
**Output:**
```
Special Character
```

---

## 21. Check if Character is Vowel or Consonant

```c
#include <stdio.h>

int main() {
    char ch = 'e';
    if (ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u' ||
        ch == 'A' || ch == 'E' || ch == 'I' || ch == 'O' || ch == 'U')
        printf("Vowel\n");
    else if ((ch >= 'A' && ch <= 'Z') || (ch >= 'a' && ch <= 'z'))
        printf("Consonant\n");
    else
        printf("Not an alphabet\n");
    return 0;
}
```
**Output:**
```
Vowel
```

---

## 22. Leap Year or Not

```c
#include <stdio.h>

int main() {
    int year = 2024;
    if ((year % 4 == 0 && year % 100 != 0) || (year % 400 == 0))
        printf("Leap Year\n");
    else
        printf("Not a Leap Year\n");
    return 0;
}
```
**Output:**
```
Leap Year
```

---

## 23. Triangle Validation Using Sides

```c
#include <stdio.h>

int main() {
    int a = 5, b = 7, c = 10;
    if (a + b > c && a + c > b && b + c > a)
        printf("Valid Triangle (by sides)\n");
    else
        printf("Invalid Triangle (by sides)\n");
    return 0;
}
```
**Output:**
```
Valid Triangle (by sides)
```

---

## 24. Triangle Validation Using Angles

```c
#include <stdio.h>

int main() {
    int angle1 = 60, angle2 = 60, angle3 = 60;
    if (angle1 + angle2 + angle3 == 180 && angle1 > 0 && angle2 > 0 && angle3 > 0)
        printf("Valid Triangle (by angles)\n");
    else
        printf("Invalid Triangle (by angles)\n");
    return 0;
}
```
**Output:**
```
Valid Triangle (by angles)
```

---

## 25. Ticket Price Discount Based on Age

```c
#include <stdio.h>

int main() {
    int age = 12;
    float price = 100, final_price;
    if (age <= 12)
        final_price = price * 0.5; // 50% discount
    else if (age >= 60)
        final_price = price * 0.7; // 30% discount
    else
        final_price = price;
    printf("Ticket Price = %.2f\n", final_price);
    return 0;
}
```
**Output:**
```
Ticket Price = 50.00
```

---

## 26. Eligible to Vote

```c
#include <stdio.h>

int main() {
    int age = 18;
    if (age >= 18)
        printf("Eligible to Vote\n");
    else
        printf("Not Eligible to Vote\n");
    return 0;
}
```
**Output:**
```
Eligible to Vote
```

---

## 27. Check Uppercase or Lowercase

```c
#include <stdio.h>

int main() {
    char ch = 'G';
    if (ch >= 'A' && ch <= 'Z')
        printf("Uppercase\n");
    else if (ch >= 'a' && ch <= 'z')
        printf("Lowercase\n");
    else
        printf("Not an alphabet\n");
    return 0;
}
```
**Output:**
```
Uppercase
```

---
