## Summary

Arrays have O(1)O(1)-time lookups. But you need enough uninterrupted space in RAM to store the whole array. And the array items need to be the same size.


But if your array stores pointers to the actual array items (like we did with our list of baby names), you can get around both those weaknesses. You can store each array item wherever there's space in RAM, and the array items can be different sizes. The tradeoff is that now your array is slower because it's not cache-friendly.


Another problem with arrays is you have to specify their sizes ahead of time. There are two ways to get around this: dynamic arrays and linked lists. Linked lists have faster appends and prepends than dynamic arrays, but dynamic arrays have faster lookups.


Fast lookups are really useful, especially if you can look things up not just by indices (0, 1, 2, 3, etc.) but by arbitrary keys ("lies", "foes"...any string). That's what hash tables are for. The only problem with hash tables is they have to deal with hash collisions, which means some lookups could be a bit slow.

## Each data structure has tradeoffs. You can't have it all.


So you have to know what's important in the problem you're working on. What does your data structure need to do quickly? Is it lookups by index? Is it appends or prepends?


Once you know what's important, you can pick the data structure that does it best.
