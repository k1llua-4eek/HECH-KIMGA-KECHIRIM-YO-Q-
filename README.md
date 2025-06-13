menu = ["lagmon","osh","shashlik","somsa","choy"]
buyurtmalar = []

if buyurtmalar:
for taom in buyurtmalar:
if taom in menu:
print(f"Menuda {taom} bor")
else:
print(f"Kechirasiz, menuda {taom} yo'q")
else:
print("Savatchangiz bo'sh!")

menu = ["lagmon","osh","shashlik","somsa","choy"]
buyurtmalar = []
narx = 0
x = int(input("Hurmatli mijoz, nechta taom buyurasiz:\t"))
for i in range(0,x):
buyurtma = input(f"{i+1}-buyurtmani kiriting:\t")
buyurtma = buyurtma.strip()
buyurtma = buyurtma.lower()
buyurtmalar.append(buyurtma)

if buyurtmalar:
for taom in buyurtmalar:
if taom in menu:
print(f"\nSizning {taom.title()} nomli buyurtmangiz qabul qilindi!")
else:
print(f"Sizning {taom.title()} nomli buyurtmangiz mavjud emas!")

else:
print("Savatchangiz bo'sh!")

for a in buyurtmalar:
if a == "osh":
narx += 20_000
if a == "somsa":
narx += 5_000
if a == "shashlik":
narx += 15_000
if a == "lagmon":
narx += 25_000
if a == "choy":
narx += 3_000

print(f"\nSizning buyurtmalar soningiz: {len(buyurtmalar)}")
print(f"Sizning to'lovingiz: {narx}")
