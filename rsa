import math
import sys

def factorize(n):
    for i in range(2, int(math.sqrt(n))+1):
        if n % i == 0:
            return (i, n//i)
    return None

if __name__ == "__main__":
    filename = sys.argv[1]
    with open(filename, "r") as f:
        for line in f:
            n = int(line.strip())
            factors = factorize(n)
            if factors is not None:
                print(f"{n}={factors[0]}*{factors[1]}")
