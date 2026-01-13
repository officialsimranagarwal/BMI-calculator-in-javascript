# BMI Calculator in JavaScript ⚖️

![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![DOM](https://img.shields.io/badge/DOM-Manipulation-orange?style=for-the-badge)

## 📖 Overview

A lightweight, client-side **Body Mass Index (BMI) Calculator**. This project demonstrates core DOM manipulation and JavaScript event handling concepts to perform real-time health metrics calculations.

## 💻 Technical Implementation

### Event Handling
The application utilizes the `window.onload` lifecycle method to ensure the DOM is fully ready before attaching event listeners.
-   **Listener**: `button.addEventListener("click", calculateBMI)`
-   **Trigger**: Captures user click events on the submit button.

### Logic Flow (`calculateBMI`)
1.  **Input Parsing**:
    -   Inputs are fetched via `document.querySelector("#id").value`.
    -   Values are typecast using `parseInt()` to ensure numerical operations.
    -   *Tech Note*: This prevents string concatenation errors during the BMI calculation.

2.  **Validation**:
    -   Checks for empty strings (`""`) or non-numeric inputs (`isNaN()`).
    -   Provides immediate feedback via innerHTML updates if validation fails.

3.  **Calculation Algorithm**:
    -   The formula used is: $BMI = \frac{Weight}{(Height/100)^2}$ (where Height is converted from cm to meters).
    -   Precision is managed using `.toFixed(2)` to limit the output to two decimal places.

4.  **Health Categorization**:
    conditional logic maps the raw BMI value to standard health categories:
    -   **Underweight**: values < 18.6
    -   **Normal**: 18.6 <= values < 24.9
    -   **Overweight**: values > 24.9

## 📂 File Structure

-   `index.html`: Structure and input forms.
-   `bmi.js`: Core logic and event handling.
-   `style.css`: Visual styling (assumed linked).

## 🚀 Getting Started

To run this project locally:
1.  Clone the repository:
    ```bash
    git clone https://github.com/officialsimranagarwal/BMI-calculator-in-javascript.git
    ```
2.  Open `index.html` in any modern web browser (Chrome, Firefox, Safari).

## 🤝 Contributing

Contributions are welcome! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for details.

## 👤 Author

**Simran Agarwal**
-   [Profile](https://github.com/officialsimranagarwal)
-   [LinkedIn](https://linkedin.com/in/simran-agarwal-54751b191)

---
*Generated with ❤️ by Simran Agarwal*
