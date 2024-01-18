# FIBONACCI-GENERATOR
def generateFibonacciSequence():
    n2 = 1
    n3 = 1
    while True:
        n1 = n2
        n2 = n3
        n3 = n1 + n2
        yield n1


a = generateFibonacciSequence()
# we generate the first 80 Fibonacci numbers
for i in range(80):
    print(next(a), end=' ')
