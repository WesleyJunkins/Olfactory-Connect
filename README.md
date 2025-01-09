# Installation for MacOS

## 1. Install XCode
1. Install XCode from the App Store. This will add XCode command line tools.
    **Alternatively**, if you don't want to install XCode, you can install the command line tools separately. Open a terminal and type:
    ```bash
    xcode-select --install
    ```
2. Follow the installation instructions.

## 2. Install Homebrew
1. Open a terminal window and paste:
    ```bash
    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
    ```
2. Follow the instructions and restart the terminal after Homebrew is installed.

## 3. Install Dependencies
1. In a terminal, paste:
    ```bash
    brew install openssl readline sqlite3 xz zlib
    ```

## 4. Install `pyenv`
1. Open a terminal window and paste:
    ```bash
    brew install pyenv
    ```

## 5. Check Your Current Python Version
1. In a terminal, type:
    ```bash
    which python
    ```
2. If it says `python not found`, type:
    ```bash
    which python3
    ```

## 6. Install Python Version 3.9.6
1. Type:
    ```bash
    pyenv install 3.9.6
    ```
2. Let the installation complete.

## 7. Confirm the New Python Version
1. Type:
    ```bash
    pyenv versions
    ```
2. Ensure that `3.9.6` is listed.

## 8. Switch to the Downloaded Python Version
1. In a terminal, navigate to the project directory and type:
    ```bash
    pyenv local 3.9.6
    ```

## 9. Create a Virtual Environment
Since a specific version of Python is required, keep this version and its libraries in the project directory instead of installing them system-wide through `pip`.
1. In the project directory terminal, type:
    ```bash
    python -m venv venv
    ```
    This creates a new Python virtual environment named `venv`.
2. Source the Python virtual environment:
    ```bash
    source venv/bin/activate
    ```

## 10. Run the Program and Install Extra Dependencies
1. Run the program once to see if any dependencies need to be installed:
    ```bash
    python Olfactory\ Connect.py
    ```
2. If the output alerts you to missing dependencies, install them using:
    ```bash
    pip install <dependency name>
    ```
3. After installing each dependency, run the program again. Ensure the robot is connected to the computer via the USB Bluetooth dongle before running the program.

## 11. When Finished
1. Close the virtual environment
    ```bash
    deactivate
    ```