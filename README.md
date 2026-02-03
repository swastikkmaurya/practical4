# practical4
Aim: Study of set in a Python

Theory : Theory: Python Sets and Frozensets
In Python, a Set is a built-in data type used to store collections of data. It is defined by three primary characteristics:

Unordered: The items do not have a defined order; they may appear in a different order every time you use them and cannot be referred to by an index.

Unchangeable: While you cannot change the items once added, you can remove items and add new ones.

Unique: Sets do not allow duplicate values. If a duplicate is added, it is automatically ignored.

Set Operations

Python sets support mathematical set theory operations, which are highly efficient for data comparison:

Union (∪): Combines all elements from both sets.

Intersection (∩): Returns only the elements present in both sets.

Difference ($- $): Returns elements present in the first set but not the second.

Symmetric Difference (Δ): Returns elements present in either set, but not both.

Frozensets

A frozenset is an immutable version of a Python set. Once created, elements cannot be added, removed, or modified. This makes them "hashable," meaning they can be used as keys in a dictionary or as elements of another set.

Algorithms:

Set Creation & Uniqueness: Initialize a collection using curly braces or set() to store unique, unordered elements.

Membership Testing: Use the in keyword to check for the existence of an element with O(1) average time complexity.

Modification: Use .add() to insert a single element or .remove()/.discard() to delete specific items from the set.

Union Operation: Combine all unique elements from multiple sets into one using the | operator.

Intersection Operation: Identify and extract only those elements that exist across all compared sets using the & operator.

Difference Operation: Subtract the elements of a subtrahend set from a minuend set using the - operator.

Symmetric Difference: Keep only the elements that are unique to each set (excluding the overlap) using the ^ operator.

Frozenset Implementation: Wrap a set in the frozenset() constructor to lock its state and prevent any further modification.

Problem 1 (Uniqueness): Cast the participant list into a set object to automatically collapse multiple registrations into single entries.

Problem 2 (Commonality): Apply the intersection operator (&) across all three student sets to find the overlap of elective subjects.

Problem 3 (Exclusivity): Calculate the intersection for "both clubs" and the symmetric difference for "exactly one club."

Problem 4 (Absence): Subtract the "present" set from the "total" set to isolate the remaining "absent" elements.

Problem 5 (Entry Removal): Invoke the .discard() method to remove a specific invalid key without triggering an error if the key is missing.

Conclusion :
This experiment demonstrates that Python Sets are a powerful and efficient tool for handling collections of unique data where order is irrelevant. Through the implementation of various problem statements, we conclude that:

Efficiency: Sets are highly optimized for membership testing (in operator) and removing duplicates compared to lists, making them ideal for large-scale data filtering like participant registration.

Mathematical Utility: The built-in operators for Union, Intersection, and Difference allow for complex logical comparisons (like finding common elective subjects or identifying absent students) to be performed with concise, readable code.
