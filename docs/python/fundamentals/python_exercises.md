**Perform below multi line assignment in a single line.**

``` md
n = 0.125
m = "abc"
z = False
```

??? example annotate "Solution"

    ``` py
    n, m, z = 0.125, "abc", False
    print(n)
    print(m)
    print(z)
    ```

<!-- end of question -->


**String exercises**

- Create a string `Hello, World!`
- Just print `,` from the string
- Get the characters from position 2 to position 5 (not included)
- Print only the characters at even position
- Replace `"H"` with `"Y"`
- Split 'My name is Rajdeep' to a list of substrings
- Remove any whitespace from beginning or end of `" Hello, World! "`
- Combine a list of strings `["ab", "cd", "ef"]` with an empty string delimitor

??? example annotate "Solution"

    ``` py
    print('\n1. Create a string `Hello, World!`')
    my_str = "Hello, World!"
    print(my_str)


    print('\n2. Just print `,` from the string')
    print(my_str[5])


    print('\n3. Get the characters from position 2 to position 5 (not included)')
    print(my_str[1:5])


    print('\n4. Print only the characters at even position')
    print(my_str[::2])


    print('\n5. Replace `"H"` with `"Y"`')
    print(my_str.replace("H", "Y"))


    print('\n6. Split "My name is Rajdeep" to a list of substrings')
    my_str = "My name is Rajdeep"
    print(my_str.split())


    print('\n7. Remove any whitespace from beginning or end of `" Hello, World! "`')
    my_str = " Hello, World! "
    print(my_str.strip())


    print('\n8. Combine a list of strings `["ab", "cd", "ef"]` with an empty string delimitor')
    str_list = ["ab", "cd", "ef"]
    print(" ".join(str_list))
    ```

<!-- end of question -->


**List exercises**

- Create a list of names containing `"John", "Alice", "Sarah", "Rajna", "George"` using list() constructor
- Print number of items in the list
- Print `"Alice", "Sarah", Rajna` from the list
- Retrieve `"George"`
- Retrieve `"Sarah"`
- Replace `"John"` with `"Jenny"`
- Replace `"Jenny", "Alice"` with `"John", "Maya"`
- Add `"Simon"`
- Add `"Betty"` before `"Sarah"`
- Remove `"John"`
- Remove element at index 2
- Remove the last element
- Add list `fruits = ["apple", "banana", "cherry", "kiwi"]` to names
- From `fruits = ["apple", "banana", "cherry", "kiwi"]`, print all fruits that has `a` in its name using list comprehension
- Reverse the order of list `fruits = ["apple", "banana", "cherry", "kiwi"]`
- Sort list numerically `num = [100, 50, 65, 82, 23]`
- Sort above list in descending order
- Join fruits and num list to a new list
- Clear fruits list
- Delete num list

??? example annotate "Solution"

    ``` py
    print('\n1. Create a list of names containing `"John", "Alice", "Sarah", "Rajna", "George"` using list() constructor\n')
    names = list(("John", "Alice", "Sarah", "Rajna", "George"))
    print(names)

    names = list()
    names.append("John")
    names.append("Alice")
    names.append("Sarah")
    names.append("Rajna")
    names.append("George")
    print(names)


    print('\n2. Print number of items in the list\n')
    print(f"No of items: {len(names)}")


    print('\n3. Print `"Alice", "Sarah", Rajna` from the list\n')
    print(names[1:4])


    print('\n4. Retrieve `"George"`\n')
    print(names[-1])


    print('\n5. Retrieve `"Sarah"`\n')
    print(names[2])


    print('\n6. Replace `"John"` with `"Jenny"`\n')
    names[0] = "Jenny"
    print(names)


    print('\n7. Replace `"Jenny", "Alice"` with `"John", "Maya"`\n')
    names[0:2] = ["John", "Maya"]
    print(names)


    print('\n8. Add `"Simon"`\n')
    names.append("Simon")
    print(names)


    print('\n9. Add `"Betty"` before `"Sarah"`\n')
    names.insert(2, "Betty")
    print(names)


    print('\n10. Remove `"John"`\n')
    names.remove("John")
    print(names)


    print('\n11. Remove element at index 2\n')
    names = ['Maya', 'Betty', 'Sarah', 'Rajna', 'George', 'Simon']
    names.remove(names[2])
    print(names)

    names = ['Maya', 'Betty', 'Sarah', 'Rajna', 'George', 'Simon']
    names.pop(2)
    print(names)


    print('\n12. Remove the last element\n')
    names.pop()
    print(names)


    print('\n13. Add list `fruits = ["apple", "banana", "cherry", "kiwi"]` to names\n')
    fruits = ["apple", "banana", "cherry", "kiwi"]
    names.extend(fruits)
    print(names)


    print('\n14. From `fruits = ["apple", "banana", "cherry", "kiwi"]`, print all fruits that has `a` in its name using list comprehension\n')
    fruits = ["apple", "banana", "cherry", "kiwi"]
    print([fruit for fruit in fruits if "a" in fruit])


    print('\n15. Reverse the order of list `fruits = ["apple", "banana", "cherry", "kiwi"]`\n')
    fruits.reverse()
    print(fruits)

    fruits.sort(reverse=True)
    print(fruits)


    print('\n16. Sort list numerically `num = [100, 50, 65, 82, 23]`\n')
    num = [100, 50, 65, 82, 23]
    num.sort()
    print(num)


    print('\n17. Sort above list in descending order\n')
    num = [100, 50, 65, 82, 23]
    num.sort(reverse=True)
    print(num)


    print('\n18. Join fruits and num list to a new list\n')
    new_list = fruits + num
    print(new_list)


    print('\n19. Clear fruits list\n')
    print(fruits)
    fruits.clear()
    print(fruits)


    print('\n20. Delete num list\n')
    print(num)
    del num
    print(num)
    ```

<!-- end of question -->


**Tuple exercises**

- Create a tuple of names`"John", "Sarah", "Alice"` using tuple() constructor
- Create a tuple of single name `"Maya"`
- Add name to names
- Retrieve `"Sarah"`
- Add `"Simon"`
- Rmove `"John"`
- Is there any workaround for add and remove?
- Unpack tuple `fruits = ("apple", "banana", "kiwi")` as per their color and print their values
- Delete fruits tuple

??? example annotate "Solution"

    ``` py
    print('\n1. Create a tuple of names`"John", "Sarah", "Alice"` using tuple() constructor\n')
    names = tuple(("John", "Sarah", "Alice"))
    print(names)


    print('\n2. Create a tuple of single name `"Maya"`\n')
    name = ("Maya",)
    print(name)


    print('\n3. Add name to names\n')
    names += name
    print(names)


    print('\n4. Retrieve `"Sarah"`\n')
    print(names[1])


    print('\n5. Add `"Simon"``\n')
    print("Cannot add items to a Tuple as it is immutable\n")


    print('\n6. Rmove `"John"`\n')
    print("Cannot remove items from a Tuple as it is immutable\n")


    print('\nIs there any workaround for add and remove?\n')
    print(names)
    names = list(names)
    names.append("Simon")
    print(tuple(names))

    names = list(names)
    names.remove("Simon")
    print(tuple(names))


    print('\n7. Unpack tuple `fruits = ("apple", "banana", "cherry")` as per their color and print their values\n')
    fruits = ("apple", "banana", "cherry")
    green, yellow, red = fruits
    print(f"Green : {green}")
    print(f"Yellow : {yellow}")
    print(f"Red : {red}")


    print('\n8. Delete fruits tuple\n')
    print(fruits)
    del fruits
    print(fruits)
    ```

<!-- end of question -->


**Nested collections**

- Retrieve `('Eternal Sunshine of the Spotless Mind', 2004)`
- Retrieve `Eternal Sunshine of the Spotless Mind`

``` md
movies = [
    ('Eternal Sunshine of the Spotless Mind', 2004),
    ('Memento', 2000)
]
```

??? example annotate "Solution"

    ``` py
    print("1. Retrieve `('Eternal Sunshine of the Spotless Mind', 2004)`")
    print(movies[0])

    print('\n2. Retrieve `Eternal Sunshine of the Spotless Mind`')
    print(movies[0][0])
    ```

<!-- end of question -->


**Dictionary exercises**

- Create a dictionary called `student`, wherein student name is `"John Smith"` and his grades are `88, 76, 92, 85, 69`
- Print student grades
- Add student age = 14
- Print `John Smith is 14 years old and his grades are 88, 76, 92, 85, 69`    # with and without for loop
- Create a dictionary called `school` using dict() constructor with school name and location'
- Merge student dictionary with school dictionary     # check name key
- Update student age to 18
- Delete grades
- List all keys
- List all values
- List all items
- Iterate and print all keys
- Iterate and print all values
- Iterate and print both keys value pairs
- Remove `location`
- Remove last item
- Remove all items
- Delete student dictionary

??? example annotate "Solution"

    ``` py
    print('\n 1. Create a dictionary called `student`, wherein student name is `"John Smith"` and his grades are `88, 76, 92, 85, 69`')
    student = {
        "name": "John Smith",
        "grades": [88, 76, 92, 85, 69]
    }
    print(student)


    print('\n 2. Print student grades')
    print(student["grades"])


    print('\n 3. Add student age = 14')
    student["age"] = 14
    print(student)


    print('\n 4. Print `John Smith is 14 years old and his grades are 88, 76, 92, 85, 69`')
    print(f'{student["name"]} is {student["age"]} years old and his grades are {", ".join(map(str, student["grades"]))}')
    print(f"John Smith is {student['age']} years old and his grades are {' '.join(str(grade) for grade in student['grades'])}")


    print('\n 5. Create a dictionary called `school` using dict() constructor with school name and location')
    school = dict({"name": "LES", "location": "Mirik"})
    print(school)


    print('\n 6. Merge student dictionary with school dictionary     # check name key')
    student.update(school)
    print(student)

    # merge operator (|)
    student = student | school
    print(student)


    print('\n 7. Update student age to 18')
    student["age"] = 18
    print(student)


    print('\n 8. Delete grades')
    del student["grades"]
    print(student)


    print('\n 9. List all keys')
    print(student.keys())


    print('\n 10. List all values')
    print(student.values())


    print('\n 11. List all items')
    print(student.items())


    print('\n 12. Iterate and print all keys')
    for key in student.keys():
        print(key)


    print('\n 13. Iterate and print all values')
    for value in student.values():
        print(value)


    print('\n 14. Iterate and print both keys value pairs')
    for key, value in student.items():
        print(f"{key} : {value}")


    print('\n 15. Remove `location`')
    print(student.pop("location"))
    print(student)


    print('\n 16. Remove last item')
    print(f"Last item: {student.popitem()}")
    print(student)


    print('\n 17. Remove all items')
    print(student)
    student.clear()
    print(student)


    print('\n 18. Delete student dictionary')
    print(student)
    del student
    print(student)
    ```

<!-- end of question -->


**Set exercises**

- Create an empty set `set1`
- Add three items `"apple", "banana", "cherry"`
- Print `"apple"` 
- Create a second set `set2` using set() constructor with at least one common item with the first set
- Find the union, symmetric difference, and intersection of the two sets
- Add set1 and set2
- Remove `"pineapple"`
- Remove any random item
- Remove all items
- Delete set1

??? example annotate "Solution"

    ``` py
    print('\n1. Create an empty set `set1`')
    set1 = set()
    print(set1)

    print('\n2. Add three items `"apple", "banana", "cherry"`')
    set1.add("apple")
    set1.add("banana")
    set1.add("cherry")
    print(set1)

    print('\n3. Print `"apple"`')
    print("Cannot access items in a set using index or key as it is unordered")

    print('\n4. Create a second set `set2` using set() constructor with at least one common item with the first set')
    set2 = set(("apple", "mango", "pineapple"))
    print(set2)

    print('\n5. Find the union, symmetric difference, and intersection of the two sets')
    print(f"Union                   : {set1.union(set2)}")
    print(f"Symmetric difference    : {set1.symmetric_difference(set2)}")
    print(f"Intersection            : {set1.intersection(set2)}")

    print('\n6. Add set1 and set2')
    set1.update(set2)
    print(set1)

    print('\n7. Remove `"pineapple"`')
    set1.remove("pineapple")
    print(set1)

    print('\n8. Remove any random item')
    set1.pop()
    print(set1)

    print('\n9. Remove all items')
    set1.clear()
    print(set1)

    print('\n10. Delete set1')
    print(set1)
    del set1
    print(set1)
    ```

<!-- end of question -->


**deque exercises**

- Create double-ended queue `[4, 5, 6]`
- Append `7` to the right
- Append `3` to the left
- Append `[8, 9, 10]` to right
- Append `[1, 2]` to left
- Insert `-1` at index 5
- Remove element from the right end
- Remove element from the left end
- Remove `-1`
- Count the number of times `5` occurs
- Return index of `7`
- Rotate deque three times to the right
- Reverse deque

??? example annotate "Solution"

    ``` py
    print('\nCreate double-ended queue `[4, 5, 6]`.')
    from collections import deque
    dq = deque([4, 5, 6])
    print(dq)

    print('\nAppend `7` to the right')
    dq.append(7)
    print(dq)

    print('\nAppend `3` to the left')
    dq.appendleft(3)
    print(dq)

    print('\nAppend `[8, 9, 10]` to right')
    dq.extend([8, 9, 10])
    print(dq)

    print('\nAppend `[1, 2]` to left')
    dq.extendleft([1, 2])
    print(dq)

    print('\nInsert `-1` at index 5')
    dq.insert(5, -1)
    print(dq)

    print('\nRemove element from the right end')
    dq.pop()
    print(dq)

    print('\nRemove element from the left end')
    dq.popleft()

    print('\nRemove `-1`')
    dq.remove(-1)
    print(dq)

    print('\nCount the number of times `5` occurs')
    print(dq.count(5))

    print('\nReturn index of `7`')
    print(dq)
    print(dq.index(7))

    print('\nRotate deque three times to the right')
    dq.rotate(3)
    print(dq)

    print('\nReverse deque')
    dq.reverse()
    print(dq)
    ```

<!-- end of question -->
