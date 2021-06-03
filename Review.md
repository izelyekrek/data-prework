# Prework review

Hi Izel 🙋🏻‍♀️!! I am writing to give you some feedback on your prework! 🚀

### 1. Snail-and-Well

The first part of this exercise was perfecr Izel, good job!!! However, you do try the bonus exercise, what happened?? 
One tip in this exercise is:
- Iterate along the new distances list 
- Then sum the distance traveled by the snail
- Sum one day 
- Rest the night distance considering the distance reached during the day
  ```python
    well_height = 125
    advance_cm = [30, 21, 33, 77, 44, 45, 23, 45, 12, 34, 55]
    nightly_distance = 20
    snail_position = 0
    days = 0

    for i in advance_cm:
        snail_position += i
    if snail_position <= well_height:
        snail_position -= nightly_distance
        days += 1
    else: 
        snail_position
  ```

### 2. Duel-of-Sorcerers

The first part of this exercise, the logic and the code to resolve the problem are perfect. Just to get picky:

- In the exercise 3 *Using the lists of spells of both sorcerers, update variables gandalf_wins and saruman_wins to count the number of times each sorcerer wins a clash.*

    ```python
    for i in range(spells):
        if gandalf[i] > saruman[i]:
            gandalf_wins += 1
        elif gandalf[i] < saruman[i]: # it is't necesssary to write the second condition using else
            saruman_wins += 1

    # Then, you will get something lijke this: 
    for i in range(spells):
        if gandalf[i] > saruman[i]:
            gandalf_wins += 1
        else: #that's means, if the first condition is not met, then sum 1 to saruman_wins
            saruman_wins += 1
    ```
¿What happended to the bonus?   
In this exercise the key was to learn how to iterate through dictionaries. if you don't understand something about this exercise or if you want us to look at it calmly and find a time to do so. 

### 3. Bus

Good job, the exercise it is perfect! 💪🔥


### 4. Robin-Hood

The first two exercises are perfect! Let's go with the the last two:

-  *Find the point closest to the center. Calculate its distance to the center*
    ```python
    def find_distance(point):
        x, y = point
        return (x ** 2 + y ** 2) ** 0.5

    unique_points = list(set(points))

    # Assumption: the first point is the closest. 
    min_distance = find_distance(unique_points[0])
    min_points = [];

    # Comparison with the rest of points.
    for point in unique_points[1:]:
        distance = find_distance(point)
        if min_distance > distance:
            min_distance = distance
            min_points = [point]
        elif min_distance == distance:
            min_points.append(point)
            
    print (min_distance)
    print (min_points)
    ```
- *If the archery target has a radius of 9, calculate the number of arrows that won't hit the target.*
    ```python
    points_outside_target = []

    for coordinates in points:
        if (find_distance(coordinates) > 9):
            points_outside_target.append(coordinates)
    arrows_missed = len(points_outside_target)

    print (arrows_missed)
    print (points_outside_target)
    ```
If you have any doubts about this exercise tell us! 

### 5. Temperature-Processor

Nice!!! You have used list comprehensions 👏🏽, which made the code more consice, generallu more readable and will run faster. 

However... Again, what happened with the bonus??? Although they are not mandatory, it is important that we do them because they will help us to create more complex code and can be a challenge from which we will learn a lot.

### 6. Rock–Paper–Scissors

- As a detail, when we create a variable it is important that we don't use `key words` as `list`, `set`, `key`... If you want to create a variable with the name "list" you could use a low bar (or choose another name), for example:
    ```python
    list_ = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
    ```

- Let's go with the sixth exercise *Define a function that randomly returns one of the 3 gesture options.*
    ```python
    def I14(w):
        return choice(a)
    ```
    Some comments about you function:
    -  The components of the definition are: 
        - **def**	The keyword that informs Python that a function is being defined
        - **<function_name>**	A valid Python identifier that names the function
        - **<parameters>** parameters that may be passed to the function
       - **<statement(s)>**	A block of valid Python statements
    It is important that the paramater that we pass to the function, since it will be on this one on which the code that is inside the function will be applied.

        For example if yoy want to do a random choice from a list we should do: 

        ```python
        def cpu_choice (to_choice):
            return choice(to_choice)
        # when we call the function:
        gestures = ['rock', 'paper', 'scissors']
        cpu = cpu_choice(gestures)
        # cpu will be a variable with a random choice based on the gesture list. 
        ```
    
        I share with you some documentation about functions [here](https://realpython.com/defining-your-own-python-function/)

        If you want to see this exercise in more depth or if you have any doubts about the functions, let me know and we will see it together.

Well Izel, overall you did a good job, however in most cases you didn't try the bonus part. If these exercises were difficult for you, tell me, we could try to explain it in more detail. 

Cheer up and whatever you need, we are here!🔥😉
