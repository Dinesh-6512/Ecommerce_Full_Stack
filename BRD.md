# Business Requirements Document (BRD)

## 1. Project Goal & Users
Build a simple, beginner-friendly e-commerce website for purchasing products online.
- **Roles:**
  - **User (Shopper):** Browses products, manages a cart, and places orders.
  - **Admin (Store Owner):** Adds new products to the catalog.

## 2. Features

### User Features
- **Register:** Create a new customer account with email and password.
- **Login:** Authenticate and receive a session token.
- **View Products:** Browse a list of all available items (title, description, price).
- **Add to Cart:** Add items with desired quantity to the shopping cart.
- **View Cart:** See selected items, quantities, item prices, and subtotal.
- **Checkout:** Provide delivery details (full name, phone, address, city, postal code).
- **Place Order:** Convert the current cart into a placed order.
- **View My Orders:** See past orders with delivery details, item summary, and total cost.

### Admin Features
- **Add Product:** Form to create a new product (title, description, price).

## 3. Scope Exclusions (Not Included)
- No online payment gateway (cash on delivery / dummy checkout).
- No search bar or product filtering.
- No separate product details page.
- No categories or tags.
- No editing or deleting products.
- No removing items from the cart.
- No order cancellation or returns.
- No admin order management dashboard.

## 4. Main User Journey
- **User:** Register -> Login -> View products -> Add to cart -> View cart -> Checkout -> Place order -> View my orders
- **Admin:** Login -> Add product -> Verify product appears in catalog

## 5. Success Criteria
- Users can successfully register and log in to receive an authorization token.
- Catalog items display accurate titles and prices.
- Items added to cart persist for the user and calculate totals correctly.
- Order submission saves delivery details and clears the active cart.
- Order history accurately lists previously placed orders for the logged-in user.
- Admin-created products immediately appear in the product catalog.

