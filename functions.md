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
