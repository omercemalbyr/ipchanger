import os
import time
import random

def change_ip(interval):
    while True:
        new_ip = f"{random.randint(1, 255)}.{random.randint(1, 255)}.{random.randint(1, 255)}.{random.randint(1, 255)}"
        os.system(f"sudo ifconfig eth0 {new_ip}")
        print(f"IP adresi değiştirildi: {new_ip}")
        time.sleep(interval)

print("*İpChanger*")
print("1. 30 saniye")
print("2. 1 dakika")
print("3. 5 dakika")
print("4. 10 dakika")

choice = input("L�tfen bir seçim yapın (1-4): ")

if choice == "1":
    interval = 30
elif choice == "2":
    interval = 60
elif choice == "3":
    interval = 300
elif choice == "4":
    interval = 600
else:
    print("Geçersiz seçim. Program sonlandırılıyor.")
    exit()

try:
    change_ip(interval)
except KeyboardInterrupt:
    print("\nProgram sonlandırıldı.")
