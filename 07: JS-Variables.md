# JavaScript Variables

## 📌 Variables = Data Containers
JavaScript variables are **containers for storing data**.

---

## 📌 Declaring Variables
JavaScript variables can be declared in **4 ways**:

### ✅ Modern JavaScript (Recommended)
- **`let`** → Block-scoped variable (can be updated, not redeclared).  
- **`const`** → Block-scoped constant (cannot be updated or redeclared).  

### ⚠️ Older JavaScript
- **`var`** → Function-scoped variable (not recommended, can cause issues).  
- **Automatically** → Using undeclared variables (not recommended, can create global scope problems).  

---

## 📌 Example: Using `let`
```javascript
let x = 5;
let y = 6;
let z = x + y;

console.log(z); // Output: 11
