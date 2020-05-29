-   Use intention revealing names
-   Use searchable names even if they end up being long
-   "My personal preference is that single-letter names can ONLY be used as local variables inside short methods. The length of a name should correspond to the size of its scope"

-   "One difference between a smart programmer and a professional programmer is that
    the professional understands that clarity is king. Professionals use their powers for good
    and write code that others can understand.

-   "Classes and objects should have noun or noun phrase names like Customer, WikiPage,
    Account, and AddressParser. Avoid words like Manager, Processor, Data, or Info in the name
    of a class. A class name should not be a verb."

-   "Methods should have verb or verb phrase names like postPayment, deletePage, or save.
    Accessors, mutators, and predicates should be named for their value and prefixed with get,
    set, and is according to the javabean standard."

    -   employee.getName();
    -   employee.setName("brandon");
    -   if(paycheck.isPosted()) {...}

-   "Pick one word for one abstract concept and stick with it. For instance, it’s confusing to
    have fetch, retrieve, and get as equivalent methods of different classes."

    DON'T do this:

    -   employee.deleteInfo();
    -   employee.removeBirthday();
