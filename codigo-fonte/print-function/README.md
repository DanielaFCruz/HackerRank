Without using any method, the idea is to print the consecutive values of the number entered by the user.

You can't start with zero, and the list needs to be printed horizontally.

if __name__ == '__main__':
    n = int(input())
    for i in range(1, n + 1):
        print(i, end='')
