# =====================================
# PROGRAM PERULANGAN LENGKAP
# =====================================

print("=== 1. PERULANGAN FOR ===")
for i in range(1, 11):
    print("Angka:", i)

print("\n=== 2. PERULANGAN WHILE ===")
i = 1
while i <= 10:
    print("Angka:", i)
    i += 1

print("\n=== 3. PERULANGAN DO-WHILE ===")
# Python tidak memiliki do-while asli,
# sehingga disimulasikan dengan while True

i = 1
while True:
    print("Angka:", i)
    i += 1

    if i > 10:
        break

print("\n=== 4. NESTED LOOP ===")
for i in range(1, 6):
    for j in range(1, 6):
        print("*", end=" ")
    print()

print("\n=== PROGRAM SELESAI ===")
