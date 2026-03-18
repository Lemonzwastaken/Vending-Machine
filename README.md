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

A Python command-line coffee machine simulator. Order your favourite brew, insert coins, and get your change — all from the terminal.

---

## Features

- **Interactive menu** — choose from Latte, Espresso, or Cappuccino
- **Coin-based payment** — insert quarters, dimes, nickles, and pennies
- **Change calculation** — get exact change returned if you overpay
- **Resource tracking** — machine tracks water, milk, and coffee levels
- **Admin report** — view current ingredients and profit at any time
- **Pretty terminal UI** — formatted tables via `PrettyTable`

---

## Menu

| Drink      | Water  | Milk   | Coffee | Price |
|------------|--------|--------|--------|-------|
| Latte      | 200 ml | 150 ml | 24 g   | $2.50 |
| Espresso   | 50 ml  | 0 ml   | 18 g   | $1.50 |
| Cappuccino | 250 ml | 50 ml  | 24 g   | $3.00 |

---

## Getting Started

### Prerequisites

- Python 3.x
- `prettytable` library

### Installation

```bash
git clone https://github.com/your-username/coffee-machine.git
cd coffee-machine
pip install prettytable
```

### Run

```bash
python main.py
```

---

## Usage

When the machine starts, you'll be shown the menu with numbered selections.

```
+------------+------+-----------+
| Name       | Cost | Selection |
+------------+------+-----------+
| latte      | $2.5 | 1         |
| espresso   | $1.5 | 2         |
| cappuccino | $3.0 | 3         |
+------------+------+-----------+
```

**Enter a number** to select your drink, then insert coins when prompted.

### Special Commands

| Command  | Description                              |
|----------|------------------------------------------|
| `report` | View current resource levels and profit  |
| `exit`   | Turn off the machine                     |

---

## Project Structure

```
coffee-machine/
│
├── main.py           # Entry point — runs the machine loop
├── menu.py           # MenuItem and Menu classes
├── coffee_maker.py   # CoffeeMaker class — manages resources
├── money_machine.py  # MoneyMachine class — handles payments
└── art.py            # ASCII art for the UI
```

---

## How It Works

1. **Menu** displays available drinks and their prices
2. **User selects** a drink by number
3. **MoneyMachine** prompts for coins and calculates total
4. If payment is sufficient, **CoffeeMaker** checks resources and brews the drink
5. Change is returned and profit is recorded
6. User can continue or exit

---

## License

This project is open source and available under the [MIT License](LICENSE).
