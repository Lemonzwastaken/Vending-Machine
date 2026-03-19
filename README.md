# ☕ Coffee Machine

```
  ░██████    ░██████   ░██████████░██████████ ░██████████    ░███     ░███    ░███      ░██████  ░██     ░██ ░██████░███    ░██ ░██████████ 
 ░██   ░██  ░██   ░██  ░██        ░██         ░██            ░████   ░████   ░██░██    ░██   ░██ ░██     ░██   ░██  ░████   ░██ ░██         
░██        ░██     ░██ ░██        ░██         ░██            ░██░██ ░██░██  ░██  ░██  ░██        ░██     ░██   ░██  ░██░██  ░██ ░██         
░██        ░██     ░██ ░█████████ ░█████████  ░█████████     ░██ ░████ ░██ ░█████████ ░██        ░██████████   ░██  ░██ ░██ ░██ ░█████████  
░██        ░██     ░██ ░██        ░██         ░██            ░██  ░██  ░██ ░██    ░██ ░██        ░██     ░██   ░██  ░██  ░██░██ ░██         
 ░██   ░██  ░██   ░██  ░██        ░██         ░██            ░██       ░██ ░██    ░██  ░██   ░██ ░██     ░██   ░██  ░██   ░████ ░██         
  ░██████    ░██████   ░██        ░██████████ ░██████████    ░██       ░██ ░██    ░██   ░██████  ░██     ░██ ░██████░██    ░███ ░█████████  
```
---

A Python coffee machine simulator built as part of my **100 Days of Code** journey. The focus of this project was practising **Object-Oriented Programming** by splitting the logic into separate classes that each handle their own responsibility.

## What it does

Order a coffee, insert your coins, and get your change — all from the terminal. The machine tracks its own resources and will let you know if it's running low on ingredients.

## Project Structure

| File | Class | Responsibility |
|------|-------|----------------|
| `menu.py` | `Menu`, `MenuItem` | Stores drinks and their ingredients |
| `coffee_maker.py` | `CoffeeMaker` | Manages resources and brews the drink |
| `money_machine.py` | `MoneyMachine` | Handles coin input, payment, and change |
| `main.py` | — | Ties all classes together and runs the loop |

## How to Run

```bash
pip install prettytable
python main.py
```

Type `report` at any time to check ingredient levels and profit, or `exit` to turn off the machine.
---

## License

This project is COPYRIGHT PROTECTED AND MUST NOT BE USED ANYWHERE
(im kidding use it to your heart's content for anything)
