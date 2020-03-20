#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) seems to be a O(n) or O(log n^3)??? which increases runtime with increase input at the same rate (Linear) and does O(1) work per iteration. What i see is (n) used to controls the outer loop because its input affects the number of iterations.


b) idk tbh it could be O(n^c) or O(n)n the initial input is n but the input n is checked again conditionally. As the size of the input increases, the runtime or space used is will grow at the same rate.



c) O(n) O(n-1) has an upper boundary and is a super-set? and is a nested loop so the runtime is dependant (recursion) but there are unknown factor such as bunnies so we would not know how many times it would run. 

## Exercise II

-Identify the input 
    n-story building
    plenty of eggs

-Identify the output 
    determine the value of f such that the number of dropped + broken eggs is minimized

-Identify all the initial variables you may need you can always change these later
    n-story building
    plenty of eggs
    floor f or higher
    floor less than floor f
    value of f
    dropped + broken eggs

-Are you going to need a loop? 
        yes
    If you know the length use a for loop if you don't know the length use a while loop. 
        while loop probably
   
-How is your information stored? Are you using a list,dict,string…?
    maybe dictionary


proposed algorithm: 
    two parameters = 1) egg     
                     2) Floor
    However we have unknown values such as egg durability = cracking under pressure or drop rate?
    Based on that information you could determine floor conditions that would purpose a cracked egg or not with a boolean value. 

runtime complexity:
    Definitely would use a loop on the O(n) runtime complexity to minimize cracked eggs over time

Note: that being said you could work backwards since we can possibly assume a-e floors wont crack an egg? and if the floor is f or higher the egg will break...

so if we set a min and max range for each iteration we can set n if less than f egg does not get broken. Keep this number for the next iteration by assigning a max value and egg does get broken you can then use random for floors and repeat this using the max value then as a min value...

which would result in a complexity O(log n) for searching through the problem and reducing broken eggs is minimized.
