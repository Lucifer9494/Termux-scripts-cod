#!/data/data/com.termux/files/usr/bin/bash

echo "Lucifer_servic: 🔄 Termux uchun barcha kerakli paketlarni avtomatik o‘rnatish boshlanmoqda..."

# Termuxni yangilash va yangilash (avtomatik "Y" bosish)
pkg install -y && pkg update -y
pkg upgrade -y
apt-get update -y
apt-get upgrade -y

# Python va pip o‘rnatish
pkg install -y python python2 python-pip

# Pip va boshqa kutubxonalarni avtomatik o‘rnatish
pip install --upgrade pip -q
pip install wheel -q
pip install asyncio -q
pip install telethon -q
pip install colorama -q
pip install bs4 -q
pip install rsa -q
pip install requests -q
pip install pyaes -q
pip install async_generator -q
pip install aiosqlite -q
pip install licensing -q

# Termux uchun ruxsatlarni sozlash
termux-setup-storage

echo "✅ Barcha paketlar avtomatik o‘rnatildi! Dasturchi Lucifer_servic"
