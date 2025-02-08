# React Product Table

This project is built following the **Thinking in React** tutorial. It implements a **searchable and filterable product table** using **React components, state, and props**.

## How State and Props Work in This Application

### Props
- **Props** are used to pass data between components.
- The `products` array is passed from `App.jsx` to `FilterableProductTable.jsx` as a **prop**.
- `FilterableProductTable` then **passes data down** to `SearchBar.jsx` and `ProductTable.jsx` using **props**.

### State
- **State** is used for dynamic and changing values.
- `FilterableProductTable.jsx` holds **two pieces of state**:
  - `filterText`: Stores the **text entered in the search bar**.
  - `inStockOnly`: Stores **whether the checkbox is checked**.
- These state values **control what gets displayed** in `ProductTable.jsx`.
- When the **user types** in `SearchBar.jsx`, it updates **state** in `FilterableProductTable.jsx`, which **re-renders the table dynamically**.

