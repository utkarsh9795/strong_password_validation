
# Strong Password Validation

## Overview

**Strong Password Validation** is a JavaScript project designed to ensure the robustness of passwords by validating them against a set of defined criteria. This project aims to help developers integrate password strength checks in their web applications, enhancing user security and protecting sensitive information.

## Features

- **Length Check:** Ensures the password meets a minimum and maximum length requirement.
- **Uppercase Letters:** Verifies the presence of at least one uppercase letter.
- **Lowercase Letters:** Ensures at least one lowercase letter is included.
- **Numeric Characters:** Checks for at least one numeric digit.
- **Special Characters:** Validates the inclusion of special characters (e.g., `!@#$%^&*`).
- **No Spaces:** Ensures that the password does not contain any whitespace characters.

## Usage

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/strong-password-validation.git
cd strong-password-validation
```

### 2. Include the Script

You can include the password validation script in your project by linking it in your HTML file or importing it into your JavaScript code.

```html
<script src="path/to/strong-password-validation.js"></script>
```

Or import it into your JavaScript file:

```javascript
import validatePassword from './strong-password-validation.js';
```

### 3. Implement the Validation

Call the `validatePassword` function with the password string as an argument:

```javascript
const password = 'YourPassword123!';
const validationResult = validatePassword(password);

if (validationResult.isValid) {
  console.log('Password is strong!');
} else {
  console.log('Password validation failed:', validationResult.errors);
}
```

### Output

- **`isValid`**: A boolean indicating whether the password is strong.
- **`errors`**: An array of error messages detailing why the password failed validation.

## Validation Criteria

- **Minimum Length:** 8 characters
- **Maximum Length:** 20 characters
- **At least one uppercase letter**
- **At least one lowercase letter**
- **At least one number**
- **At least one special character**
- **No spaces allowed**


## Installation

To include this project in your own development environment:

1. Clone the repository.
2. Use the `validatePassword` function in your application.

## Contributing

Contributions are welcome! Feel free to submit a pull request or open an issue to suggest improvements or report bugs.


