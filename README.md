# Lab 18 - Cryptography

### Author

- **Arthur Lozano**

### Code

[Code]()

### Overview

- Today we'll be tackling a cryptographic class - the Caesar Chiper
- Devise a method to encrypt a message that can then be decrypted when supplied with the corresponding key.
- Devise a way to deciphter the encrypted message event when you do NOT have the key!

### Featured Task & Requirments

- [x] Create an **encrypt** function that takes in a plain text phrase and a numeric shift.
    - [x] the phrase will then be **shifted** that many letters.
        - E.g. encrypt(‘abc’,1) would return ‘bcd’ = E.g. encrypt(‘abc’, 10) would return ‘klm’
    - [x] shifts that exceed 26 should wrap around.
        - E.g. encrypt(‘abc’,27) would return ‘bcd’
- [x] shifts that push a letter out or range should wrap around
        - E.g. encrypt(‘zzz’,1) would return ‘aaa’
- [x] Create a **decrypt** function that takes in encrypted text and numeric shift which will restore the encrypted text back to its original form when correct key is supplied.
- [o] Create a **crack** function that will decode the cipher so that an encrypted message can be transformed into its original state WITHOUT access to the key.
- [o] Devise a method for the computer to determine if code was broken with minimal human guidance.


### Implementation Notes

- In order to accomplish a certain task you’ll need access to a **corpus** of English words.
- A search on something like **python list of english words** should get you going.

### User Acceptance Tests

The application must…

- [x] encrypt a string with a given shift
- [x] decrypt a previously encrypted string with the same shift
- [x] encryption should handle upper and lower case letters
- [x] encryption should allow non-alpha characters but ignore them, including white space
- [o] decrypt encrypted version of It was the best of times, it was the worst of times. WITHOUT knowing the shift used.
refer to supplied unit tests.

### Stretch Goals

- [o] Research the  Vigenère cipher.
- [o] Find some examples of ROT13 encrypted punchlines, spoilers, etc.
- [o] Break the code for a message written in language other than English.

### Collaboration & Credit

- [Crummy](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
- [Youtube](https://www.youtube.com/watch?v=XVv6mJpFOb0)

### Configuration

- Use `poetry` to create `caesar-cipher` project.
- Use the folder created by Poetry as the root of your project's git repository
- Refer to [Lab Submission Instructions](https://codefellows.github.io/code-401-python-guide/reference/submission-instructions/labs/) for detailed instructions.

### Collab & Credit 

- [w3resource](https://www.w3resource.com/python-exercises/string/python-data-type-string-exercise-25.php)
