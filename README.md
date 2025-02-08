# Elixir Enum.each List Modification Bug
This example demonstrates an issue when trying to modify a list within an `Enum.each` loop in Elixir.  Attempting to remove elements using `List.delete` will not change the original list because Elixir lists are immutable.  The code showcases the problem and the solution provides a correct way to achieve the desired outcome.

## Bug
The `bug.ex` file contains the erroneous attempt at modifying the list during the `Enum.each` iteration.  The original list remains unchanged after the loop completes.

## Solution
The `bugSolution.ex` file shows the correct approach using `Enum.filter` to create a new list containing only the desired elements.