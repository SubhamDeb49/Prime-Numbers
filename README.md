# Prime-Numbers
#Count special numbers between boundaries

def count_Primes_nums():
    lower = int (input())
    upper = int (input())
    ctr = 0
    
    for num in range(lower, upper+1):
        if num <= 1:
            continue
        for i in range(2, num):
            if (num % i) == 0:
                break
        else:
            ctr += 1

    return ctr


print(count_Primes_nums())
