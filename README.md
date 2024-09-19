# Setting Up axe-core in Zsh on Visual Studio Code

## Prerequisites

- **Node.js**: Install Node.js from [https://nodejs.org/en/](https://nodejs.org/en/)
- **Visual Studio Code**: Download and install [Visual Studio Code](https://code.visualstudio.com/)
- **Zsh**: Ensure Zsh is installed. If not, you can install it with:
  ```bash
  sudo apt install zsh
  ```

## Setting Up axe-core

1. Open Visual Studio Code and create a new file with the following content:
   ```bash
   #!/bin/bash
   npm install axe-core
   ```

2. Save the file as `install-axe-core.sh`.

3. Open the terminal in Visual Studio Code and run the following command:
   ```bash
   chmod +x install-axe-core.sh
   ```

4. Run the script with the following command:
   ```bash

    ./install-axe-core.sh
    ```

5. To verify that axe-core is installed, run the following command:

    ```bash
    node -e "require('axe-core')"
    ```
  
    If there are no errors, axe-core is successfully installed.
    
6. To use axe-core in your project, you can import it as follows:

    ```javascript
    const axe = require('axe-core');
    ```

## Setting Up axe-core in Zsh

1. Open the `.zshrc` file in Visual Studio Code by running the following command:

    ```bash
    code ~/.zshrc
    ```

2. Add the following line to the `.zshrc` file:

    ```bash
    export PATH=$PATH:/path/to/axe-core
    ```

    Replace `/path/to/axe-core` with the path to the `node_modules` directory where axe-core is installed.

3. Save the `.zshrc` file and restart the terminal.

4. Activate the changes by running the following command:

    ```bash
    source ~/.zshrc
    ```

5. To verify that axe-core is set up in Zsh, run the following command:

    ```bash
    axe
    ```

    If axe-core is set up correctly, you should see the axe-core help message.

  ```bash
  Usage: axe [options] <url>

  Options:
    -V, --version  output the version number
    -h, --help     display help for command
  ```



## Conclusion

You have successfully set up axe-core in Zsh on Visual Studio Code. You can now use axe-core to test the accessibility of your web applications.

