my_list = [1, 2, 3, 4, 5, 6, 3, 4, 5, 7, 6, 5, 4, 3, 4, 5, 4, 3, 'привіт', 'анаконда']
def remove_dublicates(my_list):
    return list(set(my_list))

def sort_list(my_list):
    numbers = [x for x in my_list if isinstance(x, (int, float))]
    string = [x for x in my_list if isinstance(x, str)]

    numbers.sort()
    string.sort()

    return numbers + string
unique_list = remove_dublicates(my_list)

sorted_list = sort_list(unique_list)

print(sorted_list)
