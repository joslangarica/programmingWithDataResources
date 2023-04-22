# NumPy - SciPy

Here are the 10 interesting functions in SciPy and NumPy libraries, with everyday examples in an easy and clear way, formatted in Markdown.

1. **NumPy - np.array**

The `np.array` function is used to create a NumPy array, which is a special kind of list used for mathematical and scientific operations.

*Example:* Suppose you have a list of temperatures in Celsius for a week and you want to calculate the mean or average temperature.

```
import numpy as np

temperatures = [28, 23, 25, 24, 27, 23, 25]
temp_array = np.array(temperatures)
mean_temperature = np.mean(temp_array)

print(mean_temperature)

```

1. **SciPy - scipy.optimize.curve_fit**

The `curve_fit` function finds the best-fit parameters for a given function to fit a set of data points.

*Example:* You collected data about your daily expenses for a month and want to fit a linear function that describes your spending habits.

```
from scipy.optimize import curve_fit
import numpy as np

# The linear function to fit
def linear_func(x, a, b):
    return a*x + b

# Your daily expenses for a month
expenses = np.array([25, 30, 20, 32, 28, 35, 40, 20, 30, 28, 25, 27, 35, 22, 24, 28, 33, 31, 29, 36, 40, 24, 26, 28, 30, 32, 34, 31, 25, 27])
days = np.arange(1, 31)

# Fit the linear function to your expenses
popt, _ = curve_fit(linear_func, days, expenses)

a, b = popt
print(f"Slope: {a}, Intercept: {b}")

```

1. **NumPy - np.linspace**

`np.linspace` is used to generate 'n' equally spaced numbers between a start and an endpoint.

*Example:* You want to create a list of 10 equally spaced distances between 0 and 100 meters.

```
import numpy as np

distances = np.linspace(0, 100, num=10)
print(distances)

```

1. **SciPy - scipy.interpolate.interp1d**

The `interp1d` function is used to create a function that interpolates between data points.

*Example:* You have measured the temperature at three hours of the day (6:00 AM, 12:00 PM, and 6:00 PM), and you want to know the temperature at any given moment of the day.

```
import numpy as np
from scipy.interpolate import interp1d

# Hour and corresponding temperature measurements
hours = np.array([6, 12, 18])
temperatures = np.array([22, 28, 24])

# Create the interpolating function
temperature_func = interp1d(hours, temperatures, kind='linear')

# Predict the temperature at 9:00 AM
temp_9am = temperature_func(9)
print(f"Temperature at 9:00 AM: {temp_9am}")

```

1. **NumPy - np.random.randint**

`np.random.randint` is used to generate random integers.

*Example:* You want to simulate rolling a six-sided die.

```
import numpy as np

roll = np.random.randint(1, 7)
print(f"You rolled a {roll}.")

```

1. **NumPy - np.power**

`np.power` raises an array of numbers to a certain power.

*Example:* You want to calculate the square of a list of numbers.

```
import numpy as np

numbers = [1, 2, 3, 4, 5]
squares = np.power(numbers, 2)

print(squares)

```

1. **scipy.stats.norm**

The `norm`object provides access to useful functions regarding the normal distribution, like PDF (probability density function) and CDF (cumulative density function).

*Example:* You want to calculate the probability that a person is taller than 180 cm, knowing that the average human height is 170 cm and the standard deviation is 10 cm.

```
from scipy.stats import norm

mean_height = 170
std_dev = 10

# Create a normal distribution object for height
height_dist = norm(loc=mean_height, scale=std_dev)

# Calculate the probability of being taller than 180 cm
prob_taller_than_180 = 1 - height_dist.cdf(180)

print(f"Probability of being taller than 180 cm: {prob_taller_than_180}")

```

1. **NumPy - np.dot**

`np.dot` is a function that computes the dot product of two arrays.

*Example:* You want to calculate the total price of a shopping list, knowing the quantities of items and their respective costs.

```
import numpy as np

quantities = [3, 1, 2]
prices = [5, 10, 4]

total_cost = np.dot(quantities, prices)

print(f"Total cost: {total_cost}")

```

1. **SciPy - scipy.fftpack.fftn**

The `fftn` function computes the N-dimensional discrete Fourier Transform, which is useful for signal and image processing.

*Example:* You want to analyze the frequencies present in a grayscale image.

```
import numpy as np
import scipy.fftpack
import matplotlib.pyplot as plt

# Create a random grayscale image of size 128 x 128
image = np.random.rand(128, 128)

# Compute the 2D Fourier Transform
image_fft = scipy.fftpack.fftn(image)

# Visualize the Fourier Transform
plt.imshow(np.abs(image_fft))
plt.colorbar()
plt.show()

```

1. **NumPy - np.vstack & np.hstack**

The `np.vstack` and `np.hstack` functions are used to stack arrays vertically and horizontally, respectively.

*Example:* You want to create a larger array by concatenating two smaller arrays, both vertically and horizontally.