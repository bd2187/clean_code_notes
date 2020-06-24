# Formatting

-   "You should take care that your code is nicely formatted. You should choose a set of
    simple rules that govern the format of your code, and then you should consistently apply
    those rules. If you are working on a team, then the team should agree to a single set of
    formatting rules and all members should comply. It helps to have an automated tool that
    can apply those formatting rules for you."

-   "The functionality that you create today has a good chance of changing in the next
    release, but the readability of your code will have a profound effect on all the changes
    that will ever be made. The coding style and readability set precedents that continue to
    affect maintainability and extensibility long after the original code has been changed
    beyond recognition. Your style and discipline survives, even though your code does not."

-   Newspaper Metaphor

    -   Source file should read like a newspaper
    -   Name of file should be simple and explanatory
    -   Topmost parts of the file should contain high-level logic and algorithms
    -   Details should be towards the bottom of the file

-   Variable Declarations

    -   Variables should be declared as close to their usage as possible.

-   Instance variables

    -   Should be declared at the top of the class
    -   In a well designed class, instance variable are used in most (if not all) methods in the class

-   Dependent functions

    -   If one function calls another, both functions should be vertically close
    -   If possible, the caller should be declared on top of the callee

-   Vertical Ordering
    -   Function call dependencies should point in the downward direction.
    -   A function that is called should be below the function that's calling it.
    -   Important concepts should come first. They should be expressed with the least amount of polluting detail. Lowel-level details come last.
