
# tzsmmpay-django

🚀 **tzsmmpay-django** is a Python library designed to simplify payment integration with TZSMM Pay in Django projects. With this package, you can seamlessly create and verify transactions while focusing on building your application.

---

## 📦 Features

- Easy integration with TZSMM Pay API.
- Create and verify transactions with minimal effort.
- Handles API authentication and response parsing.
- Lightweight and developer-friendly.

---

## 🔧 Installation

Install the package via pip:

```bash
pip install tzsmmpay-django
```

---

## 🚀 Usage

### 1. **Initialize the Client**
Import the `TzSmmPayClient` and initialize it with your API key:

```python
from tzsmmpay_django import TzSmmPayClient

client = TzSmmPayClient(api_key="your_api_key")
```

### 2. **Create a Transaction**
Use the `create_transaction` method to generate a transaction:

```python
response = client.create_transaction(
    cus_name="John Doe",
    cus_email="john@example.com",
    amount="100.00",
    success_url="https://example.com/success",
    cancel_url="https://example.com/cancel",
    callback_url="https://example.com/callback"
)
print(response)
```

### 3. **Verify a Transaction**
Use the `verify_transaction` method to validate a transaction by its ID:

```python
response = client.verify_transaction(trx_id="transaction_id_here")
print(response)
```

---

## 📚 Documentation

Find detailed documentation and examples on [GitHub](https://github.com/TZSMM-Pay/tzsmmpay-django).

---

## 🛠️ Methods Overview

### `create_transaction`:
- **Parameters**:
  - `cus_name`: Customer's full name (string, required).
  - `cus_email`: Customer's email address (string, required).
  - `amount`: Transaction amount (string, required).
  - `success_url`: Redirect URL for successful payment (string, required).
  - `cancel_url`: Redirect URL for canceled payment (string, required).
  - `callback_url`: Callback URL for payment notification (string, required).

### `verify_transaction`:
- **Parameters**:
  - `trx_id`: The transaction ID to verify (string, required).

---

## 🧪 Running Tests

To run the tests, navigate to the project directory and execute:

```bash
python -m unittest discover tests
```

---

## 🌟 Contributing

Contributions are welcome! If you’d like to add features or fix bugs, feel free to fork the repository and create a pull request.

1. Fork the repository.
2. Create a feature branch: `git checkout -b feature-name`.
3. Commit your changes: `git commit -m "Add new feature"`.
4. Push to the branch: `git push origin feature-name`.
5. Open a pull request.

---

## ⚠️ License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## 🤝 Support

For support or inquiries, feel free to contact us or visit [https://tzsmmpay.com](https://tzsmmpay.com).

---

## 📎 Links

- **PyPI**: [tzsmmpay-django on PyPI](https://pypi.org/project/tzsmmpay-django/)
- **GitHub**: [tzsmmpay-django on GitHub](https://github.com/TZSMM-Pay/tzsmmpay-django)
- **Website**: [https://tzsmmpay.com](https://tzsmmpay.com)
```

