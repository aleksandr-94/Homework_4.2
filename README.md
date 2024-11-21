# Homework_4.2



def sum_even_index_and_multiply(lst):
    if not lst:
        return 0
    even_index_sum = sum(lst[i] for i in range(0, len(lst), 2))
    # Умножаем сумму на последний элемент списка
    return even_index_sum * lst[-1]

assert sum_even_index_and_multiply([0, 1, 7, 2, 4, 8]) == 88, 'Test 1'
assert sum_even_index_and_multiply([1, 3, 5]) == 30, 'Test 2'
assert sum_even_index_and_multiply([6]) == 36, 'Test 3'
assert sum_even_index_and_multiply([]) == 0, 'Test 4'

print("Все тесты пройдены!")
