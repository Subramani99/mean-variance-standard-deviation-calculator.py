# mean-variance-standard-deviation-calculator.py
to calculator the mean , variance, standard deviation values
import math 
def calculate_mean(numbers):
    s = sum(numbers)
    n = len(numbers)
    mean = s / n
    return mean
    def calculate_variance(numbers):
    mean = calculate_mean(numbers)
    variance = sum((x - mean) ** 2 for x in numbers) / (len(numbers) - 1)
    return variance
def calculate_stddev(numbers):
    variance = calculate_variance(numbers)
    stddev = math.sqrt(variance)
    return stddev
numbers = [1,2,3,4,5]
mean = calculate_mean(numbers)
variance = calculate_variance(numbers)
stddev = calculate_stddev(numbers)

print("numbers:", numbers)
print("mean:", mean)
print("variance:", variance)
print("standard Deviation:", stddev)




output
numbers: [1, 2, 3, 4, 5]
mean: 3.0
variance: 2.5
standard Deviation: 1.5811388300841898



he above code defines three functions, calculate_mean, calculate_variance, and calculate_stddev. These functions take in a list of numbers as an argument and calculate the mean, variance, and standard deviation, respectively.

To use the code, simply create a list of numbers and call the appropriate function. The example above demonstrates how to use the functions with a list of numbers [1, 2, 3, 4, 5].
