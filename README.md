# 🛒 DemoShop — Selenium BDD Test Automation Framework

A Python-based UI test automation framework for the [DemoShop](https://demowebshop.tricentis.com/) web application, built with **Selenium**, **pytest**, and **pytest-bdd** following the **Page Object Model (POM)** design pattern.

---

## 📁 Project Structure

```
demoshop/
|
├── features/
|   ├── login.feature
│   ├── search.feature
│   ├── cart.feature
│   ├── checkout.feature
│   ├── order.feature
|   ├── shipping_address.feature
│   └── api.feature  
|         
├── pages/        
|   ├── base_page.py
│   ├── login_page.py
│   ├── home_page.py
│   ├── product_page.py
│   ├── cart_page.py
│   ├── checkout_page.py
│   └── order_page.py
|
├── step_definitions/ 
|   ├── login_steps.py
│   ├── search_steps.py
│   ├── cart_steps.py
│   ├── checkout_steps.py
│   └── api_steps.py
|
├── conftest.py          
├── pytest.ini           
└── requirements.txt     
```

---

## 🧰 Tech Stack

| Tool | Purpose |
|---|---|
| Python | Core language |
| Selenium | Browser automation |
| pytest | Test runner |
| pytest-bdd | BDD support with Gherkin syntax |
| WebDriver Manager | Automatic ChromeDriver management |
| python-dotenv | Environment variable management |

---

## ⚙️ Prerequisites

- Python 3.8+
- Google Chrome browser
- pip

---

## 🚀 Getting Started

**1. Clone the repository**

```bash
git clone https://github.com/kapilsengar/Selenium-Squad.git
cd Selenium-Squad
```

**2. Install dependencies**

```bash
pip install -r requirements.txt
```

**3. Run all tests**

```bash
pytest
```

**4. Run a specific feature**

```bash
pytest features/your_feature.feature
```

**5. Run with verbose output**

```bash
pytest -v
```

---

## 🧪 How It Works

Tests are written in **Gherkin** (`.feature` files inside `features/`) using Given/When/Then syntax. Each step maps to a Python function in `step_definitions/`. Browser interactions are abstracted into **Page Object** classes inside `pages/`, keeping tests clean and maintainable.

The `conftest.py` fixture spins up a maximized Chrome browser before each test and automatically quits it afterwards — no manual teardown needed.

---

## 📦 Key Dependencies

```
selenium==4.44.0
pytest==9.0.3
pytest-bdd==8.1.0
webdriver-manager==4.0.2
python-dotenv==1.2.2
```

Full list in [`requirements.txt`](./requirements.txt).

---

## 🤝 Contributing

Pull requests are welcome! Please open an issue first to discuss any major changes.

---

