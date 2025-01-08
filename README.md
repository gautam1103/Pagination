

# Product Pagination Application

This project demonstrates a simple React application that fetches a list of products from an external API and displays them with pagination functionality. It dynamically fetches, renders, and paginates product data using React hooks like `useState` and `useEffect`.

## Features

- **Fetch Products:** Retrieves product data from the DummyJSON API.
- **Display Products:** Displays products with thumbnails and titles.
- **Pagination:** Implements dynamic pagination to navigate through products in chunks of 10 per page.

---

## Installation and Setup

### Prerequisites

- Node.js installed on your system.
- Basic knowledge of React and JavaScript.

### Steps to Set Up

1. **Clone the Repository**  
   Clone this repository to your local machine:
   ```bash
   git clone https://github.com/your-repo-name.git
   cd your-repo-name
   

2. **Install Dependencies**  
   Install the required dependencies using npm or yarn:
   ```bash
   npm install
   ```
   or
   ```bash
   yarn install
   ```

3. **Start the Development Server**  
   Start the application locally:
   ```bash
   npm start
   ```
   or
   ```bash
   yarn start
   ```

4. **Access the Application**  
   Open your browser and navigate to:
   ```
   http://localhost:3000
   ```

---

## Preview

![image](https://github.com/user-attachments/assets/63e14195-be9f-4736-b249-92c4c274c7cc)

![image](https://github.com/user-attachments/assets/a3b0c400-8cc3-486f-952f-38edca9ee4f8)



## Usage

1. Upon loading, the app fetches the list of products from the DummyJSON API.
2. Products are displayed in a grid format, 10 per page.
3. Use the pagination controls (`◀`, `▶`, and page numbers) to navigate through the product list.

---

## Code Structure

### Key Components and Logic

1. **`App` Component**
   - **State Management:**
     - `products`: Stores the fetched product data.
     - `page`: Tracks the current page number.
   - **Fetching Data:**
     - Fetches product data from `https://dummyjson.com/products?limit=100`.
     - Populates the `products` state with the fetched data.
   - **Pagination Handler:**
     - Enables users to navigate between pages and update the displayed products.

2. **Pagination Logic**
   - Splits the `products` array into chunks of 10.
   - Disables pagination controls at the start and end of the list.

3. **Styling**
   - The `App.css` file is used for layout and visual styles, including pagination highlights and disabling inactive controls.

---

## API Reference

The application fetches data from the following API:

- **Endpoint:**  
  `https://dummyjson.com/products?limit=100`

- **Response Example:**
  ```json
  {
    "products": [
      {
        "id": 1,
        "title": "iPhone 9",
        "thumbnail": "https://dummyimage.com/iphone9.png"
      },
      ...
    ]
  }
  ```

---

## Styling Notes

Ensure that the following CSS classes are defined in `App.css` for proper rendering:

- `.products`: Grid container for products.
- `.products__single`: Individual product card.
- `.pagination`: Container for pagination controls.
- `.pagination__disable`: Styles for disabled pagination buttons.
- `.pagination__selected`: Styles for the selected page number.

---

## Improvements and Extensions

Consider the following enhancements:
- Add loading and error handling states during API calls.
- Implement search and filter functionality for the products.
- Make the number of products per page configurable.

---

## License

This project is licensed under the MIT License. Feel free to use, modify, and distribute this code as per the license terms.

---

## Acknowledgments

- [DummyJSON API](https://dummyjson.com/) for providing product data.
- React for the robust library enabling dynamic user interfaces.

```

