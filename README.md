***Readme***

This code helps calculate the current value for a meta goal based on how far above the road are latest datapoints across a list of goals.

 Before using, mark the list of the goals which you need to take into account with a unique tag. (It only makes sense to take into account some goals and not others. For example, it doesn't work for do-less goals. Works best for goals where the direction of data accumulation is monotonous. E.g. odometer or do-more goals where the total can only become higher and whittle-down goals where the total can only become lower. Should work fine with odometer resets.)

Set up a goal that will accept the meta values as an odometer goal. I use the rate of 0.1, just for it to be non-zero, but the rate is not important here, since the pressure will be not from this goal's rate but from the rates of all the goals that are taken into account.

The datapoint that is posted takes into account 10 goals with closest-to-the-road latest datapoints. Think of it as a score on the scale of 0 to 100, where 0 is "at least 10 goals are in the red today" and 100 as "all goals are at least 10 days ahead of the plan". In my experience, it make little sense to actually strive to achieve the 90+ range, as then the freedom to work more one this or that goal disappears. Instead, it is the journey that is the destination :)

**Add your INFO in the second cell with code.**

After the last cell, you cap see a recap confirming that the datapoint has been posted and a list of goals that you can work on that contribute to the meta goal.
