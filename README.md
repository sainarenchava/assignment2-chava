# assignment2-chava
# Sai Naren Chava
###### Home

My favourtie place is my home where my **family** is. A home is a place where i have my __heart__ and all that i adore.It Comforts me. There is nothing more important than a good, safe and secure home.

***
# Directions of travel from Maryville to Home
1. Search for flights and their deals
2. Book the fligh tickets with a perfect itineary
3. Take a cab to Kansas City International Airport
   1. Check in the bags and go through the security
   2. Check your terminal and the gate number to proceed there
   3. Hop on the flight to Dubai which is a duration of 10hrs 15 mins
4. After reaching Dubai wait for your connecting flight to Hyderabad International Airport
5. Arrive at Hyderabad International Airport after a duration of 8hrs 30 mins
   1. Go through immigration process
   2. Collect your check in bags
   3. Go through security
6. Exit the airport, take a cab for a ride home
7. Surprise your family and spend some amazing time with them.

List of items
* Stuff needed for family picnic
  * Picnic blanket
  * Corckscrew or bottle opener
  * Packing the picnic basket with food 
* Starting a garden at home
  * Gloves
  * Garden fork
  * Watering can
* Swim wear
* Camping stuff

[AboutMe](AboutMe.md)

***
# List of Food/Drinks you need to try before you die
As i am very fond of Indian cusinie over anything else, i have decided to mention four best dishes of my favourite along with the location and the cost.
| Dish | Location | Cost |
| --- | --- | ---: |
| Punugulu | Andhra | $2 |
| Biryani | Hyderabad | $10 |
| Royaala Iguru | Raayalaseema | $15 |
| Kallu | Telengana | $40 |

***
# Pithy Quotes using Markdown language
> I have only made this letter longer because I have not had the time to make it shorter. *Blaise Pascal*

> Read a thousand books and your words will flow like river. *Virginia Wolf*

***
# Data structures code fencing
> Binary Indexed Tree also called Fenwick Tree provides a way to represent an array of numbers in an array, allowing prefix sums to be calculated efficiently. For example, an array [2, 3, -1, 0, 6] is given, then the prefix sum of first 3 elements [2, 3, -1] is 2 + 3 + -1 = 4.

Link to the source <https://www.hackerearth.com/practice/data-structures/advanced-data-structures/fenwick-binary-indexed-trees/tutorial/>
```
struct FenwickTree2D {
    vector<vector<int>> bit;
    int n, m;

    // init(...) { ... }

    int sum(int x, int y) {
        int ret = 0;
        for (int i = x; i >= 0; i = (i & (i + 1)) - 1)
            for (int j = y; j >= 0; j = (j & (j + 1)) - 1)
                ret += bit[i][j];
        return ret;
    }

    void add(int x, int y, int delta) {
        for (int i = x; i < n; i = i | (i + 1))
            for (int j = y; j < m; j = j | (j + 1))
                bit[i][j] += delta;
    }
}
```
Link to the source code <https://cp-algorithms.com/data_structures/fenwick.html>