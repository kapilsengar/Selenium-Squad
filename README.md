# 🛒 DemoShop — Selenium BDD Test Automation Framework

A Python-based UI test automation framework for the [DemoShop](https://demowebshop.tricentis.com/) web application, built with **Selenium**, **pytest**, and **pytest-bdd** following the **Page Object Model (POM)** design pattern.

---

## 📁 Project Structure

```
demoshop/
|
├── features/
|   ├── add_to_cart.feature
│   ├── address_management.feature
│   ├── billing_address.feature
│   ├── contact_us.feature
│   ├── invalid_login.feature
|   ├── login.feature
|   ├── logout.feature
│   ├── order_confirmation.feature
│   ├── payment_method.feature
│   ├── product_details.feature
│   ├── product_sorting.feature
|   ├── register.feature
|   ├── remove_from_cart.feature
│   ├── search_product.feature
│   ├── shipping_address.feature
│   └── shipping_method.feature  
|         
├── pages/        
|   ├── address_page.py
│   ├── billing_address_page.py
│   ├── cart_page.py
│   ├── contact_us_page.py
│   ├── invalid_login_page.py
│   ├── login_page.py
|   ├── logout_page.py
│   ├── login_page.py
│   ├── order_confirmation_page.py
│   ├── payment_method_page.py
│   ├── product_details_page.py
|   ├── product_sorting_page.py
│   ├── register_page.py
│   ├── remove_cart_page.py
│   ├── search_page.py
│   ├── shipping_address_page.py
│   └── shipping_method_page.py
|
├── step_definitions/ 
|   ├── test_address_steps.py
│   ├── test_billing_address_steps.py
│   ├── test_cart_steps.py
│   ├── test_contact_us_steps.py
|   ├── test_invalid_login_steps.py
│   ├── test_login_steps.py
│   ├── test_logout_steps.py
│   ├── test_order_confirmation_steps.py
|   ├── test_payment_method_steps.py
│   ├── test_product_details_steps.py
│   ├── test_product_sorting_steps.py
│   ├── test_register_steps.py
|   ├── test_remove_cart_steps.py
│   ├── test_search_steps.py
│   ├── test_shipping_address_steps.py
│   └── test_shipping_method_steps.py
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

