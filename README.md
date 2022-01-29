# assignment2-venepalli
# Gopija Venepalli
###### McDonald's

**McDonald's** is best known for its hamburgers, cheeseburgers and french fries but I love to have McChicken, it's my favourite.It is surrounded by Hy-vee,El Maguey and Pizzahut in **W South Ave,Maryville**.

***

# Kansas City International Airport

1. Book a car. 
2. Take right from McDonald's.
3. It's a straight road.Go straight for an hour to reach Kansas Airport.
    1. There are three terminals A,B,C.
    2. Go to the terminal mentioned in boarding pass to reach your destination.

* Foods that I suggest are mentioned below
    * McChicken
    * Fries
    * Chicken Nuggets

**[Gopija's](AboutMe.md)**

---

## Sport Activity List

Below details are of sport activities which are going to be held at different places.You can register to particate and amount for personal equipments is also mentioned if needed.

| Name | Location | Amount
| :--- | :---: | ---: |
| Volleyball | Texas | 200 |
| Cricket | Chicago | 180 |
| Badminton | Newyork | 160 |
| Basketball | Washington DC | 170
| Football | King of Prussia | 190
| Hockey | New Jersey | 210

---

## Pithy Quotes

>The way to get started is to quit talking and begin doing.<br>-*Walt Disney*

>Believe you can and you're halfway there.<br>-*Oprah Winfrey*

>Nothing is impossible, the word itself says, ‘I'm possible!'.<br>-*Audrey Hepburn*

---

## Ternary Search Algorithm

>A ternary search algorithm is a technique in computer science for finding the minimum or maximum of a unimodal function. A ternary search determines either that the minimum or maximum cannot be in the first third of the domain or that it cannot be in the last third of the domain, then repeats on the remaining two thirds. A ternary search is an example of a divide and conquer algorithm.<br>
<https://en.wikipedia.org/wiki/Ternary_search>
```
double ternary_search(double l, double r) {
    double eps = 1e-9;              //set the error limit here
    while (r - l > eps) {
        double m1 = l + (r - l) / 3;
        double m2 = r - (r - l) / 3;
        double f1 = f(m1);          //evaluates the function at m1
        double f2 = f(m2);          //evaluates the function at m2
        if (f1 < f2)
            l = m1;
        else
            r = m2;
    }
    return f(l);                    //return the maximum of f(x) in [l, r]
}
```
<https://cp-algorithms.com/num_methods/ternary_search.html>