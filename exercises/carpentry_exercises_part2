---------------------------------------
# Writing Functions
---------------------------------------

-------------
## Exercise 1 - just discuss

What does the following program print?

```
def report(pressure):
    print('pressure is', pressure)

print('calling', report, 22.5)
```

-------------
## Exercise 2

Fill in the blanks to create a function that takes a single filename as an argument, 
loads the data in the file named by the argument, and returns the minimum value of column `gdpPercap_1972` in that data:

```
import pandas

def min_in_data(____):
    data = ____
    return ____
```

### Extension!

Apply the function `min_in_data` to all data files of the gapminder data containing `gdp` in the filename and print the output for each file.

=> named arguments...!

-------------
## Exercise 3

In mathematics, a dynamical system is a system in which a function describes the time dependence of a point in a geometrical space. 
A canonical example of a dynamical system is a system called the logistic map

https://en.wikipedia.org/wiki/Logistic_map 

1. Define a function called logistic_map that takes two inputs: x, representing the state of the system at time t, and a parameter r. 
This function should return a value representing the state of the system at time t+1.

--- pause ---

2. Using a for loop, iterate the logistic_map function defined in part 1 starting from an initial condition of 0.5 for t_final=10, 100, and 1000 periods. Store the intermediate results in a list so that after the for loop terminates you have accumulated a sequence of values representing the state of the logistic map at time t=0,1,…,t_final.


```
initial_condition = 0.5
t_final = 10
r = 1.0
trajectory = [initial_condition]
for t in range(1, t_final):
    trajectory.append(logistic_map(trajectory[t-1], r))
```

--- pause ---

3. Encapsulate the logic of your for loop into a function called iterate that takes the initial condition as its first input, the parameter t_final as its second input and the parameter r as its third input. The function should return the list of values representing the state of the logistic map at time t=0,1,…,t_final.

---------------------------------------
# Scope
---------------------------------------

-------------
## Exercise 1 - discuss


```
pressure = 103.9

def adjust(t):
    temperature = t * 1.43 / pressure
    return temperature
```

Ask for temperature outside function?


---------------------------------------
# Conditionals
---------------------------------------

-------------
## Exercise 1

Fill in the blanks so that this program creates a new list containing zeroes where the original 
list’s values were negative and ones where the original list’s values were positive:

```
original = [-1.5, 0.2, 0.4, 0.0, -1.3, 0.4]
result = ____
for value in original:
    if ____:
        result.append(0)
    else:
        ____
print(result)
```

### output:
[0, 1, 1, 1, 0, 1]


-------------
## Exercise 2

Create a function `calculate_life_quartile` with `expec` as input variable, that returns the 
number or None instead of printing it

```
expec = 63.

if expec < 58.41:
    # This observation is in the first quartile
    print(1)
elif expec >= 58.41 and expec < 67.05:
    # This observation is in the second quartile
    print(2)
elif expec >= 67.05 and expec < 71.70:
    # This observation is in the third quartile
    print(3)
elif expec >= 71.70:
    # This observation is in the fourth quartile
    print(4)
else:
    # This observation has bad data
    print(None)


```

### solution

```
def calculate_life_quartile(expec):
    if expec < 58.41:
        # This observation is in the first quartile
        return 1
    elif expec >= 58.41 and expec < 67.05:
        # This observation is in the second quartile
        return 2
    elif expec >= 67.05 and expec < 71.70:
        # This observation is in the third quartile
        return 3
    elif expec >= 71.70:
        # This observation is in the fourth quartile
        return 4
    else:
        # This observation has bad data
        return None
        
calculate_life_quartile(62.5)
```

? extension -> why is the else: return None here actually not required?

=> pandas `apply` instead of for-loop...


-------------
## Exercise 3

Modify this program so that it prints the filename and its number of records of the file that has the fewest records:

```
import glob
import pandas
fewest = ____
fewest_file = ____
for filename in glob.glob('data/*.csv'):
    dataframe = pandas.____(filename)
    ____
    ____
    ____
print('smallest file', fewest_file, 'has', fewest, 'records')
```

---------------------------------------
# Style
---------------------------------------

-------------
## Exercise 1

What type of input or the function would provide an error and why?

```
def calc_bulk_density(mass, volume):
    """Return dry bulk density = powder mass / powder volume."""
    return mass / volume
```

=> by adding `assert` you can be defensive!


-------------
## Exercise 2 - showcase

Logistic_map takes two inputs: x, representing the state of the system at time t, and a parameter r. 
This function returns a value representing the state of the system at time t+1. 
https://en.wikipedia.org/wiki/Logistic_map

```
def logistic_map(x, r):
    return r * x * (1 - x)
```

=> 

```
def logistic_map(x, r):
    """Predict next step of Logistic map model
    
    Parameters
    ----------
    x : float
        representing the state of the system at time t
    r : float
        model parameter
        
    Returns
    -------
    value representing the state of the system at time t+1
    """
    return r * x * (1 - x)
```


Optional:

a function called `iterate` takes the initial condition as its first input,
the parameter t_final as its second input and the parameter r as its third input. 
The function returns the list of values representing the state of the logistic map at time t=0,1,…,t_final.

```
def iterate(initial_condition, t_final, r):
    trajectory = [initial_condition]
    for t in range(1, t_final):
        trajectory.append(logistic_map(trajectory[t-1], r))
    return trajectory
```

DOCUMENT!

