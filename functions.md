# Functions

-   Write small functions
    -   public static String renderPageWithSetupsAndTeardowns(
        PageData pageData, boolean isSuite)
        throws Exception {
        if (isTestPage(pageData))
        includeSetupAndTeardownPages(pageData, isSuite);
        return pageData.getHtml();
        }
-   FUNCTIONS SHOULD DO ONE THING. THEY SHOULD DO IT WELL.
    THEY SHOULD DO IT ONLY.

-   Function arguments: "The ideal number of arguments for a function is
    zero (niladic). Next comes one (monadic), followed
    closely by two (dyadic). Three arguments (triadic)
    should be avoided where possible. More than three
    (polyadic) requires very special justification—and
    then shouldn’t be used anyway."

-   Flag Arguments

    -   Flag arguments are ugly. Passing a boolean into a function is a truly terrible practice.
        It immediately complicates the signature of the method, loudly proclaiming that this function
        does more than one thing. It does one thing if the flag is true and another if the flag is false!

-   Try to avoid side effects

    -   Don't do this:
        function checkPassword(username, password) {
        // decrypt password

            // initialize session if password is valid

        }

-   Output arguments

    -   In general output arguments should be avoided. If your function must change the state
        of something, have it change the state of its owning object.

        -   appendFooter(s);
            public void appendFooter(StringBuffer report)

        -   much of the need for output arguments disappears in OO languages because this is intended to act as an output argument. In other words, it would be better for appendFooter to be invoked as: report.appendFooter();

-   Functions should either do something or answer something, but not both. Either your
    function should change the state of an object, or it should return some information about
    that object. Doing both often leads to confusion.

-   Extract Try/Catch Blocks

    -   They confuse the structure of the code and mix normal processing with error processing
    -   Tip: Extract try/catch logic into functions of their own
        function deletePage(page) {
        try {
        deletePageAndAllReferences(page)
        } catch(err) {
        logError(err)
        }
        }

    function deletePageAndAllReferences(page) {
    // delete page
    }

    function logError(err) {
    // log error
    }

-   "Functions should do one thing. Error handing is one thing. Thus, a function that handles
    errors should do nothing else. This implies (as in the example above) that if the keyword
    try exists in a function, it should be the very first word in the function and that there
    should be nothing after the catch/finally blocks."

-   "Writing software is like any other kind of writing. When you write a paper or an article,
    you get your thoughts down first, then you massage it until it reads well. The first draft
    might be clumsy and disorganized, so you wordsmith it and restructure it and refine it until
    it reads the way you want it to read.
    When I write functions, they come out long and complicated. They have lots of
    indenting and nested loops. They have long argument lists. The names are arbitrary, and
    there is duplicated code. But I also have a suite of unit tests that cover every one of those
    clumsy lines of code.
    So then I massage and refine that code, splitting out functions, changing names, eliminating duplication. I shrink the methods and reorder them. Sometimes I break out whole
    classes, all the while keeping the tests passing.
    In the end, I wind up with functions that follow the rules I’ve laid down in this chapter.
    I don’t write them that way to start. I don’t think anyone could."

-   "Master programmers think of systems as stories to be told rather than programs to
    be written. They use the facilities of their chosen programming language to construct a
    much richer and more expressive language that can be used to tell that story. Part of that
    domain-specific language is the hierarchy of functions that describe all the actions that
    take place within that system. In an artful act of recursion those actions are written to
    use the very domain-specific language they define to tell their own small part of the
    story.
    This chapter has been about the mechanics of writing functions well. If you follow
    the rules herein, your functions will be short, well named, and nicely organized."
