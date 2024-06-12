# Random Password Generator

## Project Description
The Random Password Generator is a simple Python project that generates a random password based on a specified length. The password includes uppercase letters, lowercase letters, numbers, and special characters to ensure strong security.

## Features
- Generates a random password of user-defined length.
- Includes a mix of uppercase letters, lowercase letters, numbers, and special characters.
- Ensures strong and secure passwords for various uses.

## Requirements
- Python 3.x

## How to Run the Project
1. Ensure you have Python 3.x installed on your system.
2. Download or clone the project files to your local machine.
3. Open a terminal or command prompt and navigate to the directory containing the `random_password_generator.py` file.
4. Run the script by typing:
   ```bash
   python random_password_generator.py
   ```
5. Enter the desired length of the password when prompted.
6. The generated password will be displayed on the screen.

## Code Explanation
The script for the Random Password Generator is straightforward and consists of the following steps:

1. Import the `random` module to utilize its random sampling functionality.
   ```python
   import random
   ```

2. Define a string containing all possible characters for the password, including uppercase letters, lowercase letters, numbers, and special characters.
   ```python
   password = "ABCDEFGHIJKLMNOPQRSTUVWXYZ1234567890abcdefghijklmnopqrstuvwxyz!@#$%^&*()_+}{:"
   ```

3. Prompt the user to enter the desired length of the password.
   ```python
   length_password = int(input("Enter the length of the password: "))
   ```

4. Generate the password by randomly sampling the specified number of characters from the defined character set and joining them into a single string.
   ```python
   a = "".join(random.sample(password, length_password))
   ```

5. Print the generated password to the screen.
   ```python
   print(f"The generated password is: {a}")
   ```

## Example
```bash
Enter the length of the password: 12
The generated password is: A9@7m!Jf&2Xh
```

## Notes
- The length of the password must be less than or equal to the number of unique characters available in the `password` string (68 characters).
- If you enter a length greater than 68, the script will raise a `ValueError` due to the nature of `random.sample`.

## License
This project is open-source and available under the MIT License. Feel free to use, modify, and distribute the code.

## Contributing
Contributions are welcome! If you have any suggestions or improvements, please submit a pull request or open an issue.

## Contact
If you have any questions or need further assistance, feel free to contact the project maintainer at omkarkadle@gmail.com.

---

Enjoy generating strong and secure passwords with the Random Password Generator!
