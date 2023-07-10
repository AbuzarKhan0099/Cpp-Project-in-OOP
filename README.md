
## Online Shopping System / Grocery System

This C++ project represents an online shopping system or grocery system implemented using object-oriented programming (OOP) principles. The project provides separate functionalities for administrators and users.

### Features

#### Admin Functionality:
- Add Product: Allows administrators to add new products to the system by providing product details such as code, name, price, and discount percentage.
- Remove Product: Enables administrators to remove a product from the system based on its product code.
- Modify Product: Allows administrators to update the details of an existing product, such as its code, name, price, and discount percentage.
- List All Products: Displays a list of all products available in the system, including their product code, name, price, and discount percentage.
- Remove All Data: Removes all product data from the system, providing administrators with a clean slate.
- View Purchasing History: Allows administrators to view the purchase history, which provides information about the products purchased and the total grand amount.

#### User Functionality:
- List All Products: Displays a list of all products available in the system, including their product code, name, price, and discount percentage.
- Purchase Product: Enables users to select a product by its product code and specify the desired quantity for purchase. The system calculates the actual price and applies the discount based on the product's details. It then generates a receipt displaying the product details, quantity, price, actual price, discount, and total price. The system also maintains a purchase history file.

### Project Structure

The project consists of the following classes:

- `Shopping`: A base class that provides common functionality related to product listing.
- `Admin`: Derived from the `Shopping` class, this class represents the administrative functionality, allowing administrators to add, remove, modify, and list products. It also provides options to remove all data and view the purchasing history.
- `User`: Derived from the `Shopping` class, this class represents the user functionality, allowing users to list all products and make purchases.
 
The project utilizes file handling to store and retrieve product data from the `database.txt` file. It also maintains a `purchase_history.txt` file to record the purchase history.

### Usage

1. The main menu presents two options: "Admin" and "User." Choose the appropriate option by entering `1` for Admin or `2` for User.
2. For the Admin menu, various options are available, including adding, removing, modifying, and listing products. Administrators can also remove all data or view the purchasing history.
3. For the User menu, users can list all products or purchase products by specifying the product code and quantity. The system calculates the total price based on the product's actual price and discount.
4. The system generates a receipt displaying the product details, quantity, price, actual price, discount, and total price. The grand total of all purchases is accumulated and displayed at the end of the receipt.
5. The system maintains a purchase history file, `purchase_history.txt`, which records the details of each purchase.

### Dependencies

The project relies on the following C++ libraries:
- iostream: Provides standard input/output functionality.
- fstream: Enables reading from and writing to files.
- vector: Provides a dynamic array to store product-related data.
- sstream: Facilitates reading from and writing to strings using stream operators.

### Future Improvements

To further enhance this project, you could consider implementing additional features such as user authentication, searching and filtering products, sorting products by price or name, and adding error handling for input validation.

Please note that the provided description is based solely on the given code snippet. If there are additional features or functionalities in the complete project, you can incorporate them into the description accordingly.
