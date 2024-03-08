# Minimum-number-of-Shovels
Raj urgently needs to buy a shovel. He finds the right one in a store where each shovel is priced at k rupees. The store has an unlimited supply of these shovels.  Raj carries an endless number of "10- rupee coins" and exactly one coin worth r rupees (where 1 ≤ r ≤ 9) in his pocket.

def minimum_shovels(k, r):
    for i in range(1, 11):
        total_cost = i * k  
        if total_cost % 10 == 0 or total_cost % 10 == r:
            return i 

k, r = map(int, input().split())

result = minimum_shovels(k, r)
print(result)
