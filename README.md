
# 🛒 Blazor CRUD Product Management System

<div align="center">

<img src="https://img.shields.io/badge/Project-Type: CRUD Dashboard-blue?style=for-the-badge" />
<img src="https://img.shields.io/badge/Framework-Blazor Server-purple?style=for-the-badge&logo=dotnet" />
<img src="https://img.shields.io/badge/Language-C Sharp-lightgrey?style=for-the-badge&logo=csharp" />
<img src="https://img.shields.io/badge/UI-QuickGrid + Bootstrap-success?style=for-the-badge&logo=bootstrap" />
<img src="https://img.shields.io/badge/Database-Entity Framework Core-green?style=for-the-badge&logo=sqlite" />

</div>

---

## 📦 Project Overview

This is a **CRUD Web Application** built with **Blazor Server** that allows users to **Create**, **Read**, **Update**, and **Delete** products using a clean and responsive UI powered by **QuickGrid** and styled with a modern dark theme.

The app connects to a database using **Entity Framework Core**, making it a perfect example of full-stack development using C#, Razor Components, and SQL-backed models.

---

## ✨ Features

- 🔍 View all products in a **QuickGrid** table
- ➕ Add new products
- ✏️ Edit product details
- 📄 View full product information
- 🗑️ Delete products with confirmation
- 📦 Product properties include:
  - `Name`
  - `Description`
  - `Price`
  - `Quantity`

---

## 🧱 Tech Stack

| Technology              | Purpose                                |
|------------------------|----------------------------------------|
| **Blazor Server (.NET 6+)** | UI Framework (Razor Components)      |
| **Entity Framework Core**   | ORM for database operations         |
| **QuickGrid**           | Modern data grid UI for listing items |
| **Bootstrap 5 (Dark Theme)** | Clean and modern responsive styling  |
| **C# / Razor / LINQ**   | Backend logic and UI binding          |
| **SQL Server / SQLite** (Configurable) | Database layer           |

---

## 🗂 File Structure Overview

```plaintext
/Pages
│
├── Index.razor           # Product list (QuickGrid)
├── Create.razor          # Create product form
├── Edit.razor            # Edit product form
├── Details.razor         # View product info
├── Delete.razor          # Confirm and delete
│
/Models
│   └── Products.cs       # Product data model
/Data
│   └── CRUDTASKContext.cs # EF DB context (not shown above)
````

---

## 📄 Sample Model – `Products.cs`

```csharp
public class Products
{
    public int Id { get; set; }
    public string Name { get; set; } = string.Empty;
    public string Description { get; set; } = string.Empty;
    public decimal Price { get; set; }
    public int Quantity { get; set; }
}
```

---

## 🔄 CRUD Screens Summary

### 🏠 `/products` – Product Dashboard

* Displays all products in a responsive dark-themed `QuickGrid`
* Links to edit, view, and delete

### ➕ `/products/create`

* Form to add a new product with data validation

### ✏️ `/products/edit?id={id}`

* Form to edit a product by ID

### 🔍 `/products/details?id={id}`

* Full product info view in styled card layout

### 🗑️ `/products/delete?id={id}`

* Confirmation screen before deleting product

---

## 🧪 Data Validation

All forms use:

* `<DataAnnotationsValidator />`
* `<ValidationMessage />` per field
* Required and range checks can be added with `[Required]`, `[Range]`, etc. in the model.

---

## ✅ To Run This Project

> Make sure you have [.NET SDK 6+](https://dotnet.microsoft.com/download) installed.

```bash
# Step 1: Clone this repo
git clone https://github.com/your-username/blazor-crud-products.git
cd blazor-crud-products

# Step 2: Restore dependencies and run
dotnet restore
dotnet run
```

The app will launch at `https://localhost:5001` or `http://localhost:5000`.

---

## 👨‍💻 Developed By

**Muhammad Saad Khan**
📧 [saado652004@gmail.com](mailto:saado652004@gmail.com)
🔗 GitHub: [@saadoxyz](https://github.com/saadoxyz)

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=00C853&height=120&section=footer&text=CRUD+Mastery+with+Blazor!&fontColor=ffffff&fontSize=30" />

</div>
```

---
