# MHDDOS ДЛЯ ![Android](https://img.shields.io/badge/-Android-090909?style=for-the-badge&logo=android&logoColor=47C5FB)
### УВАГА! TERMUX ВСТАНОВЛЕННИЙ У GOOGLE PLAY ДЛЯ ANDROID 11+ НЕ ПІДІЙТЕ (БІЛЬШЕ НЕ ПІДТРИМУЄТЬСЯ І БУДУТЬ ПОМИЛКИ)
- За наступним посиланням скачуємо і встановлюємо [Termux](https://archive.org/details/termux-app_v0.118.0github-debug_universal)
- Заходимо в Termux і водимо команди:
```termux
apt update && upgrade -y
pkg install python -y && pkg install rust -y && pkg install git -y
pip install --upgrade pip
cd ~
export CARD_BUILD_TABGET=aarch64-linux-android
termux-setup-storage
cd ~/storage/shared
rm -rf mhddos_proxy
git config --global --add safe.directory /storage/emulator/0
git clone https://github.com/porthole-ascend-cinnamon/mhddos_proxy.git
cd mhddos_proxy
pip install -r termux_requirements.txt
```
- Запуск атаки:
Відркиваємо Termux:
Заходимо в папку mhddos_proxy
```termux
cd ~/storage/shared/mhddos_proxy

  