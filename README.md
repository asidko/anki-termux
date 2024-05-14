# anki-termux

# At the moment, it will install: Anki v24.04.1 (ccd9ca1a) Python 3.11.2 PyQt 6.4.2

# Required packages
sudo apt install python3 python3-pip python-is-python3 python3-venv python3-pyqt5 pyqt5-dev-tools python3-pyqt6.qt{quick,webengine,multimedia}

# Additional packages for fonts and media
sudo apt install mpv ibus-data fonts-noto-color-emoji

# Install Anki
pip install --upgrade pip --break-system-packages
pip install --upgrade --pre aqt --break-system-packages

# Run Anki
env QTWEBENGINE_CHROMIUM_FLAGS="--disable-gpu" QTWEBENGINE_DISABLE_SANDBOX=1 anki
