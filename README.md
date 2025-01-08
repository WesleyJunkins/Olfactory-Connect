Installation for MacOS

1. Install XCode from the app store. This will add XCode command line tools.
    A. Alternatively, if you don't want to install XCode, you can install the command line tools separately. Open a terminal and type:
        xcode-select --install
    B. Follow the installation instructions.

2. Install homebrew.
    A. Open a terminal window and paste:
        /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
    B. Follow the instructions and restart the terminal after homebrew is installed.

3. Install some dependencies.
    A. In a terminal, paste:
        brew install openssl readline sqlite3 xz zlib

3. Install pyenv. This allows us to easily manage multiple versions of Python, which is useful because this software uses dependencies that only work on older versions of python.
    A. Open a terminal window and paste:
        homebrew install pyenv

4. See which version of Python you are currently using.
    A. In a terminal, type:
        which python
    B. If it says 'python not found', type:
        which python3

5. We need python version <<<FIND VERSION LATER>>>

6. Confirm that the new python version was downloaded.
    A. Type: pyenv versions
    B. Ensure that <<<FIND VERSION LATER>>> is listed.

7. Switch to the downloaded version.
