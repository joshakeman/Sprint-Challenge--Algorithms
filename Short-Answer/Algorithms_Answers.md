Add your answers to the Algorithms exercises here.

I.

a) n^3
b) n^4
c) n

II.

This sounds like a problem that could be solved with binary search, which has a worst-case time complexity of O(log n).

The search algorithm would start at the middle floor (n // 2) and drop an egg. If it breaks, you know it will also break on all floors above that point, so you can eliminate all those floors from your search. If the egg does not break, on the other hand, you know that it will not break on any of the floors below you either, so you can eliminate those floors and continue looking only in the half above you for that first floor where the egg does break. WIth this style of search you effectively cut n in half on each step, which is why the time complexity is log n.