# Caesar Cipher
## About Code
Python implementation of a basic Caesar cipher encryption and decryption tool with an interactive user interface. Let's go through the code step by step and explain its functionality:

1. The code starts by defining the lowercase English alphabet using the `alphabet` list.

2. The `encryption(plain_text, shift_key)` function takes the `plain_text` (message to be encrypted) and a `shift_key` as input and performs the encryption process using the Caesar cipher algorithm. It shifts each lowercase letter in the `plain_text` by the specified `shift_key` positions and builds the `cipher_text` accordingly. Non-alphabet characters remain unchanged. The resulting `cipher_text` is then printed.

3. The `decryption(cipher_text, shift_key)` function is similar to the encryption function, but it performs the decryption process using the Caesar cipher algorithm. It shifts each lowercase letter in the `cipher_text` back to its original position using the specified `shift_key` and builds the `plain_text` accordingly. Non-alphabet characters remain unchanged. The resulting `plain_text` is then printed.

4. The code sets the initial value of the `wanna_end` variable to `False`.

5. It enters a `while` loop, which will repeatedly execute the code block as long as `wanna_end` is `False`.

6. Inside the loop, the user is prompted to input their choice between encryption and decryption using the `input()` function. The user's choice is stored in the `what_to_do` variable.

7. The user is then asked to enter the message they want to process (either for encryption or decryption). The input is converted to lowercase using the `lower()` method and stored in the `text` variable.

8. Next, the user is asked to enter the shift key (the number of positions to shift the letters) as an integer. The input is stored in the `shift` variable.

9. Depending on the user's choice (`what_to_do`), the code calls the corresponding function (`encryption` or `decryption`) with the provided message and shift key as arguments.

10. After the encryption or decryption is performed, the user is asked if they want to continue using the tool or exit the program. The input is stored in the `play_again` variable.

11. If the user chooses to exit (`play_again == 'no'`), the code sets `wanna_end` to `True`, which will break out of the loop, effectively ending the program. A farewell message is printed before the program terminates.

Overall, the code provides a user-friendly command-line interface for encrypting and decrypting messages using the Caesar cipher technique. It allows users to repeatedly perform these operations until they decide to end the program by typing 'no' when prompted to continue.
