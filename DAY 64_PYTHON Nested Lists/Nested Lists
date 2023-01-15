table={}
for _ in range(int(input())):
    name = input()
    score = float(input())
    if score not in table:
        table[score]=[name]
    else:
        table[score].append(name)
del table[min(table)]
for i in sorted(table[min(table)]):
    print(i)