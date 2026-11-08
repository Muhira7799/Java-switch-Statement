# Java `switch` Statement Example

A minimal Java program that demonstrates how a `switch` statement works by printing the name of a weekday from a number.

## What It Demonstrates

- Choosing between several cases with `switch`
- Ending each case with `break`
- Using `default` when no case matches

```java
int day = 4;

switch (day) {
    case 1:
        System.out.println("monday");
        break;
    case 2:
        System.out.println("Tuseday");
        break;
    case 3:
        System.out.println("wednesday");
        break;
    case 4:
        System.out.println("Thursday");
        break;
    default:
        System.out.println("No Case is matching the expression");
}
```

## How It Works

1. `day` is set to `4`.
2. `switch` compares `day` with each `case` value in order.
3. `case 4` matches, so it prints `Thursday`.
4. `break` stops the switch, so the remaining cases are skipped.
5. If `day` matched none of the cases, `default` would run instead.

## Output

```
Thursday
```

| `day` value | Output |
|-------------|--------|
| 1 | monday |
| 2 | Tuseday |
| 3 | wednesday |
| 4 | Thursday |
| Anything else | No Case is matching the expression |

## Requirements

- Java Development Kit (JDK) 8 or higher

## Getting Started

### Clone the repository

```bash
git clone https://github.com/<your-username>/<your-repo-name>.git
cd <your-repo-name>
```

### Compile

```bash
javac SwitchCase.java
```

### Run

```bash
java SwitchCase
```

## Why `break` Matters

Without `break`, Java continues running the next cases too (called fall-through). If you remove the `break` after `case 4`, the program would also run the `default` code and print both messages.

## Try It Yourself

- Change `day` to `2` or `9` and run the program again
- Add cases 5 to 7 for the rest of the week
- Remove a `break` and observe the fall-through

## Project Structure

```
.
├── SwitchCase.java
└── README.md
```

## Next Steps

- Use a `String` in the `switch` instead of an `int`
- Try the newer arrow syntax (`case 1 -> ...`) in Java 14 and above
- Compare `switch` with an `if / else if` chain
