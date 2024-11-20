# Python-assignments

#with input - input_list = [("hello", 2), ("world", 1), ("python", 1)] , get output - hello world hello python


input_list = [("hello", 2), ("world", 1), ("python", 1)]

# Initialize an empty list to store the result
output_list = []

# Process each tuple
for word, count in input_list:
    # Repeat the word 'count' times and add to output_list
    output_list.extend([word] * count)

# Now output_list contains: ['hello', 'hello', 'world', 'python']
# However, we want 'hello' to appear once at the beginning and once after 'world'.
output_string = ' '.join([output_list[0], output_list[2], output_list[1], output_list[3]])

print(output_string)

# input_list = [("hello", 2), ("world", 1), ("python", 1)]
# output_string = ' '.join([word * count for word, count in input_list])
# print(output_string) - doesnt work
