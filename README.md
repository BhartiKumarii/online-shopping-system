# 🛒 Online Shopping System

A terminal-based Online Shopping System built with **Python** and **MySQL** as a Class 12 final project. It simulates a real-world shopping experience with both a customer interface and an admin management panel.

---

## 📌 Features

### 👤 Customer
- Register and login with mobile number and password
- Browse products by category:
  - 📱 Mobiles (OnePlus, Redmi, Samsung, Realme, Apple)
  - 📺 TVs & Electric Appliances (Smart TV, AC, Washing Machine, Refrigerator)
  - 👗 Women's Fashion (Ethnic Wear, Western Wear)
  - 👔 Men's Fashion (Shirts, T-Shirts, Jeans, Shoes)
- Add items to cart
- Place and cancel orders
- Choose payment mode (COD, UPI, Card, EMI, Net Banking)
- View and edit account details

### 🔐 Admin
- Secure admin login
- Add, update, or delete products and categories
- View all customer details
- View all payment/order records
- Edit admin account details

---

## 🛠️ Tech Stack

| Technology | Usage |
|---|---|
| Python 3.x | Core application logic |
| MySQL | Database for products, users, orders |
| mysql-connector-python | Python-MySQL connection |
| tabulate | Formatted table display in terminal |

---

## 📂 Project Structure

```
online-shopping/
│
├── online-shopping.py     # Main application file
├── onlinestore.sql        # MySQL database schema and data
├── requirements.txt       # Python dependencies
├── .gitignore             # Files to ignore in Git
├── synopsis.pdf           # Project synopsis document
└── README.md              # Project documentation
```

---

## ⚙️ Setup & Installation

### 1. Clone the repository
```bash
git clone https://github.com/BhartiKumarii/online-shopping.git
cd online-shopping
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Set up the MySQL database
- Open MySQL and run the provided SQL file:
```bash
mysql -u root -p < onlinestore.sql
```

### 4. Configure database credentials
Open `online-shopping.py` and update the connection details:
```python
conn = c.connect(
    host="localhost",
    username="your_mysql_username",
    password="your_mysql_password",
    database="newdb"
)
```

> 💡 **Tip for future:** Use a `.env` file to store credentials securely instead of hardcoding them.

### 5. Run the application
```bash
python online-shopping.py
```

---

## 🗄️ Database Tables

| Table | Description |
|---|---|
| `customer` | Stores customer details |
| `admin` | Stores admin credentials |
| `products` | Product catalog |
| `category` | Product categories |
| `cart_item` | Items added to cart by customers |
| `orders` | Placed orders with payment info |
| `information` | Brand/product information |

---

## 📸 Sample Output

```
*** VERIFIED SUCCESSFULLY ***

__________ THE ONLINE SHOPPING SYSTEM __________

=================You want to search for=================

1.MOBILES
2.TV'S & ELECTRIC APPLIANCES
3.WOMEN'S FASHION
4.MEN'S FASHION
```

---

## 📝 Note

This project was developed as a **Class 12 Computer Science final project**. It demonstrates:
- Python programming fundamentals
- MySQL database connectivity using `mysql-connector-python`
- Real-world application logic like login, cart, and order management

---

## 👩‍💻 Author

**Bharti Kumari**  
GitHub: [@BhartiKumarii](https://github.com/BhartiKumarii)

---

## 📄 License

This project is open source and available for educational purposes.
