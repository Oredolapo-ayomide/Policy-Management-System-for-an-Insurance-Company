# Policy Management System for an Insurance Company

## Overview

This project simulates a **Policy Management System** for an insurance company. It is designed to help policy managers:
- Register, suspend, and reactivate policyholders.
- Create, update, and suspend insurance products.
- Manage and track payments including penalties and reminders.

This system is built using **Object-Oriented Programming** principles in Python and consists of three main classes:
- `Policyholder`
- `Product`
- `Payment`

Each class is placed in a separate `.py` file for modularity and clarity.

---

## Project Structure

```

policy\_management\_system/
│
├── policyholder.py                 # Class for managing policyholders
├── product.py                      # Class for insurance products
├── payment.py                      # Class for payment processing
├── policyholder_demonstration.py  # Main file to demonstrate functionality

````
---

## Requirements

- Python 3.8 or higher

---

## How to Use

### 1. **Download the Project**

* download the ZIP file and unzip it on your computer.

---

### 2. **Run the Demonstration Script**

```bash
python policyholder_demonstration.py
```

This will:

* Create two insurance products
* Register two policyholders
* Add payments to their accounts
* Print out their full account details (products purchased and payments made)

---

## Class Breakdown

### `Policyholder` (`policyholder.py`)

Manages policyholder registration, suspension, reactivation, and keeps track of associated products and payments.

**Key Methods:**

* `suspend()` – Suspend the policyholder's account.
* `reactivate()` – Reactivate the account.
* `add_policy(product)` – Add a policy/product to the holder.
* `add_payment(payment)` – Add a payment.
* `get_details()` – Returns a dictionary of all policyholder data.

---

### `Product` (`product.py`)

Handles product creation, updates, and suspension.

**Attributes:**

* `product_id`, `product_name`, `premium`, `status`

**Key Methods:**

* `update(new_name, new_premium)` – Modify product details.
* `suspend()` – Deactivate product.

---

### `Payment` (`payment.py`)

Tracks individual payments made by policyholders.

**Attributes:**

* `policy_id`, `amount`, `date`, `status`

**Key Methods:**

* `add_penalty(penalty_amount)` – Increases the amount due.
* `send_reminder()` – Sends a payment reminder.

---

## Demonstration

The demonstration is found in `policyholder_demonstration.py`. It shows:

* Product creation
* Policyholder registration
* Payment processing
* Detail output

---
