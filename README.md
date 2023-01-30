# python-function-programs
1. """Write a Python program to create a lambda function that adds 15 to a given number passed in as an argument, 
also create a lambda function that multiplies argument x with argument y and print the result
"""
n = lambda x: x+15
print(n(20))
m= lambda x,y: x*y
print(m(11,22))


2. #Write a Python program to sort a list of tuples using Lambda.
l = [('English', 88), ('Science', 90), ('Maths', 97), ('Social sciences', 82)]

print(sorted(l,key=lambda x :(x[1])))


#Write a Python program to sort a list of dictionaries using Lambda on the basis of color
l1= [{'make': 'Nokia', 'model': 216, 'color': 'Black'}, {'make': 'Mi Max', 'model': 2, 'color': 'Gold'}, {'make': 'Samsung', 'model': 7, 'color': 'Blue'}]
print(sorted(l1,key=lambda k:k['color']))
print(sorted(l1,key=lambda k:k['model']))
print(sorted(l1,key=lambda k:k['make']))


3. Write a Python program to find intersection of two given arrays using Lambda
a1=[1, 2, 3, 5, 7, 8, 9, 10]
a2=[1, 2, 4, 8, 9]

#print(list(filter(lambda x:a1[int(x)] in a2[int(x)],(a1,a2))))
result=lambda a,b:[x for x in a if x in b]
print(result(a1,a2))
