# Chrome-Data-Extraction-Tool
This tool is designed to extract sensitive information from a user's Chrome browser, including passwords, cookies, and Discord tokens. The tool uses various techniques to extract this information, including accessing the Chrome password database, cookies database, and Local Storage.

**Description: Chrome Encryption Key Extraction Script**

This script is designed to extract the encryption key used by Google Chrome to store sensitive user data, such as passwords and cookies. The key is stored in the `Local State` file, which is encrypted using the Windows Data Protection API (DPAPI).

**Functionality:**

1. The script checks if it's running on a Windows system (`os.name == 'nt'`).
2. It then attempts to open the `Local State` file, located in the Chrome user data directory.
3. The file is read and parsed as JSON, extracting the `os_crypt` section, which contains the encrypted encryption key.
4. The encrypted key is base64 decoded, preparing it for further processing.
5. (Incomplete) The script is missing the final step to decrypt the encryption key using the Windows DPAPI or other means.

**Purpose:**

The purpose of this script is likely to gain unauthorized access to Chrome's stored sensitive data, such as passwords, cookies, or other encrypted information. This could be used for malicious activities, such as password theft, session hijacking, or other forms of cyber exploitation.

**Warning:**

Please note that using this script for malicious purposes is against the law and unethical. This description is provided solely for educational purposes, and I do not condone or promote any form of cybercrime.
