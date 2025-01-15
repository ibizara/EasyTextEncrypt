# How to Use

This application provides a simple interface for encrypting and decrypting text using AES-256 in CBC mode.

A **live demo** is available at [https://ibizara.github.io/EasyTextEncrypt/](https://ibizara.github.io/EasyTextEncrypt/). 

Below are detailed instructions on how to use the various features of the application.

## 1. Encrypt

To encrypt a string, fill in the following fields:

| Field                | Description                                                                 |
| -------------------- | --------------------------------------------------------------------------- |
| Text                 | Text you wish to encrypt, e.g. "My secret recipe - Butter and Sugar".       |
| Passphrase           | Passphrase to encrypt the text with, e.g. "mysecretpassword".               |
| Reference (optional) | Optional reference for the encryption, e.g. "Kitchen".                      |

Click the "Encrypt" button to generate the encrypted string and other related fields.

## 2. Decrypt

To decrypt an encrypted string, the following fields are required:

| Field                | Description                                                                                             |
| -------------------- | ------------------------------------------------------------------------------------------------------- |
| Encrypted Text       | Encrypted string in base-64, e.g. "CnMdaWr5jkdru22pwWoQiUsJbXTVYFmDK0xjbToD2zsVkQO8Lx2hjDVJ93jPMhkl".   |
| Passphrase           | Passphrase used to encrypt the string, e.g. "mysecretpassword".                                         |
| IV                   | Initialization vector used for added uniqueness, e.g. "2fc6a34cbd04f703d759714e0d612d28".               |
| Salt                 | Salt used during encryption, e.g. "f6363dc612e98ccbb6480bb8e58b1c0d".                                   |

Click the "Decrypt" button to reveal the original text.

## 3. Other

Additional features and fields:

| Field                | Description                                                                 |
| -------------------- | --------------------------------------------------------------------------- |
| URI Encoded String   | A string that can be used to populate fields.                               |
| Decrypted Text       | Output based on the provided encrypted text, IV, salt, and passphrase.      |
| Initialization Vector (IV) | Automatically generated during encryption for added security.         |
| Salt                 | Automatically generated during encryption for key derivation.               |
| Generated Key        | Derived key based on the passphrase and salt.                               |
| URI Input            | Paste the full URI encoded string here to populate all relevant fields.     |

## Example Usage

1. **Encrypt:**
    - Text: "My secret recipe - Butter and Sugar"
    - Passphrase: "mysecretpassword"
    - Reference: "Kitchen" (optional)

    Click "Encrypt" to generate the encrypted string, IV, salt, and URI encoded string.

2. **Decrypt:**
    - Encrypted Text: "CnMdaWr5jkdru22pwWoQiUsJbXTVYFmDK0xjbToD2zsVkQO8Lx2hjDVJ93jPMhkl"
    - Passphrase: "mysecretpassword"
    - IV: "2fc6a34cbd04f703d759714e0d612d28"
    - Salt: "f6363dc612e98ccbb6480bb8e58b1c0d"

    Click "Decrypt" to reveal the original text.

## Buttons

- **Encrypt**: Encrypt the provided text using the given passphrase.
- **Decrypt**: Decrypt the provided encrypted text using the given passphrase, IV, and salt.
- **Show Advanced**: Toggle the visibility of advanced fields (IV, salt, generated key, encrypted text).
- **Clear**: Clear all input and output fields in the form.
- **Copy to Clipboard**: Copy the URI encoded string to the clipboard.

## Pasting a URI

You can paste a URI encoded string into the "URI Encoded String" field, and the application will automatically populate the relevant fields.

This application ensures the security and integrity of your data using AES-256 encryption in CBC mode, providing both confidentiality and uniqueness for each encryption operation.
