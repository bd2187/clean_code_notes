# Comments

-   "The proper use of comments is to compensate for our failure to express ourself in
    code. Note that I used the word failure. I meant it. Comments are always failures. We must
    have them because we cannot always figure out how to express ourselves without them,
    but their use is not a cause for celebration.
    So when you find yourself in a position where you need to write a comment, think it
    through and see whether there isn’t some way to turn the tables and express yourself in
    code. Every time you express yourself in code, you should pat yourself on the back. Every
    time you write a comment, you should grimace and feel the failure of your ability of
    expression."

-   Clear and expressive code with few comments is far superior to cluttered and complex
    code with lots of comments. Rather than spend your time writing the comments that
    explain the mess you’ve made, spend it cleaning that mess.

    -   // Check to see if the employee is eligible for full benefits
        if ((employee.flags & HOURLY_FLAG) &&
        (employee.age > 65))
    -   if (employee.isEligibleForFullBenefits())

-   Noisy comments - redundant - "Replace the temptation to create noise with the determination to clean your code. You’ll
    find it makes you a better and happier programmer."

-   Commented out code

    -   Others who see that commented-out code won’t have the courage to delete it. They’ll think it is there for a reason and is too important to delete.

-   If you must write a comment, then make sure it describes the code it appears near. Don’t
    offer systemwide information in the context of a local comment.
