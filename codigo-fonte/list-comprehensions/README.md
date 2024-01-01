# All in one line of code.

new_list = expression for item in iterable if condition

- expression: is a expression that be avaliable and insert in new list.
- item: is a variable that represents each element in the iterable (e.g., a list, a range, etc.).
- iterable: It is the sequence of elements that you will traverse.
- condition (optional): This is a conditional expression that determines whether the item will be included in a new list or not.

I've created a new list [new_list] to store all combinations of i, j and k at intervals (![[Pasted image 20231231081640.png]]), where the sum of these items is not equal to n.

# Without the List Comprehensions: 

if __name__ == '__main__':
    x = int(input())
    y = int(input())
    z = int(input())
    n = int(input())

	new_list = []
		for i in range (x + 1)
			for j in range (y + 1)
			    for k in range (z + 1)
					 if i + j + k != n
					 new_list.append([i, j, k])
print(new_list)

Obs.: The Append method in Python is used to add an element to the end of a list.

# With o List Comprehensions:

if __name__ == '__main__':
    x = int(input())
    y = int(input())
    z = int(input())
    n = int(input())
    
new_list = [[i, j, k] for i in range (x+1)  for j in range (y+1) for k in range (z+1) if (i+j+k) !=n ]

print(new_list)