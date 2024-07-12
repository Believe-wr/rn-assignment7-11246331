# rn-assignment7-11246331

# E-Commerce Mobile App
## Overview
This e-commerce mobile application is built using React Native and provides a seamless shopping experience for users. The app features a product list, detailed product views, and a shopping cart. It incorporates a drawer menu for easy navigation and persistent data storage using AsyncStorage.

# Design Choices
## User Interface
1. Header Navigation: The header includes a menu icon, a logo, and icons for search and cart functionalities. This keeps the main navigation elements accessible at all times.
2. Drawer Menu: The drawer menu provides quick access to different, sections of the app such as Store, Locations, Blog, Jewelry, Electronic, and Clothing.
3. Product List: A grid layout displays products, each featuring an image, title, description, and price. Users can navigate to detailed product views by tapping on any product.
4. Fixed Bottom Button: The "Add to Basket" button is fixed at the bottom of the product detail screen, ensuring easy access regardless of the scroll position.
## Data Storage
AsyncStorage: The app uses AsyncStorage to persist the shopping cart data. This ensures the cart's state is retained even when the app is closed and reopened.

# Screens
## HomeScreen
Displays a list of products with the ability to add products to the cart and navigate to the product detail screen.
## ProductDetailScreen
Shows detailed information about a selected product.
## CartScreen
Displays the list of products added to the cart.

# Implementation
## Data Fetching
The app fetches product data from an external API (https://fakestoreapi.com/products). This is handled using fetch within useEffect hooks to ensure data is loaded when the component mounts.
## State Management
1. useState: React's useState is used for managing local states such as the cart and the list of products.
2. useEffect: useEffect is used for side effects like fetching data and loading cart items from AsyncStorage.
Persistent Storage
3. Loading Cart: The cart is loaded from AsyncStorage when the app initializes. This is done using an async function within a useEffect hook.
4. Adding to Cart: When a product is added to the cart, the new cart state is saved to AsyncStorage. This ensures that the cart data is persisted between sessions.

# Screenshots
## HomeScreen
![WhatsApp Image 2024-07-12 at 08 58 11_bfcbf720](https://github.com/user-attachments/assets/d45eadd7-f2ea-44f0-b768-8fceae29f828)
![WhatsApp Image 2024-07-12 at 08 58 11_d637a66f](https://github.com/user-attachments/assets/ae1c39f3-8e4a-42e8-9d6c-441523ec4b4b)

## ProductDetailScreen
![WhatsApp Image 2024-07-12 at 08 58 11_d9e5e3ec](https://github.com/user-attachments/assets/d758b3b5-24ea-4e3d-b28b-ff693cf98d46)
![WhatsApp Image 2024-07-12 at 08 58 10_9d2411c2](https://github.com/user-attachments/assets/41c02de7-977b-4a63-afa2-73c4391b9a78)

## CartScreen
 ![checkout](https://github.com/user-attachments/assets/bd416809-d9f0-4688-92ef-c9c275f90283)

