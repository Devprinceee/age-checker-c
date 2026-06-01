# age-checker-c
# Age Classifier in C

A simple C program that determines whether a user is an adult, a teenager, or a child based on the age they input.

## Features
- Accepts user input for age.
- Uses conditional logic (`if-else` statements) to classify the age group.
- Outputs the category: **adult**, **teenagers**, or **child**.

## Age Classification Rules
- **Adult**: Age 18 or above ($\ge 18$)
- **Teenager**: Age between 14 and 17 ($> 13$ and $< 18$)
- **Child**: Age 13 or below

## How to Run

### Prerequisites
You need a GCC compiler installed on your system.  
Ex:- Turmux & linux

### Steps  
1. pkg update && pkg upgrade
2. pkg install git
3. pkg install clang

   
5. **Clone the repository** (or copy the code):
   ```bash
   git clone https://github.com/Devprinceee/age-checker-c
   cd age-checker-c
   ```

2. **Compile the program**:
   ```bash
   gcc age-checker.c -o age-checker
   ```

3. **Run the executable**:
   - On Windows:
     ```cmd
     age-checker.exe
     ```
   - On Linux/Mac:
     ```bash
     ./age-checker
     ```

## Code Preview
```c
#include<stdio.h>

int main() {
    int age;
    printf("Enter age: ");
    scanf("%d", &age);

    if(age >= 18) {
        printf("adult");
    } 
    else if(age > 13 && age < 18) {
        printf("teenagers");
    } 
    else {
        printf("child");
    }

    return 0;
}
```
## Author - Prince kumar ✨

## License
This project is open-source and available under the [MIT License](LICENSE).
