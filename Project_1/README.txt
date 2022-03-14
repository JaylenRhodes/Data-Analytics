Down Function
    I made it very simple with a just an if-else statemenet to represent the yardage return.
    Random number is made, if the random number is greater than the success then play fails otherwise return a range within our tuple yardrange

Drive Function
    Initialize with a variable I called downCalls to keep track of the downs, I tried using Count at first but it seems to no longer be supported by newer Python versions
    Made a for loop within the range of 4 since we know that they can not exceed 4 downs
    Within the loop yards for a touchdown are subtracted every iteration according to our yardsreturned and downcalls get added 1
    If the yards to TD are less than or equal to 0, then scored and print accordingly for the pointattempt compared to the percentage of success
    Else if downCalls is 4 then no points
    else i + 1 to iterate through

Drive Depicted Function
    Same as drive but I printed within each value of i to represent the current downCalls
    Yards from their endzone is 100 - yards to a touchdown and yards to touchdown is just our already tracked argument

Simulate Game Function
    Unfortunately, I couldn't solve this one no matter the modifcations I made
    I went through and reworked all of my functions to see if anything changed
    I can almost guarantee that the reason being that it can't print the scores appropriately is due to my downCalls variable
    In order to solve that though, I would have to rework everything again and I am limited on time and frustrated
    As for what I did
    Initialized the variables to whatever was required
    Created a for loop witin the range of the number of inputted drives
    If i is less than or equal to the number of drives then I assigned the results of drive to some new variables for each team
    Once everything is assigned accordingly, then add it to each score for every iteration and add 1 to I
    Else simply exit the loop
    This seems like the most logical approach to satisfy what was needed but I've no idea how to modify it print the appropriate results