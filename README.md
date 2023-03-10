# Module-14-Machine-Learning-Trading-Bot
Algorithmic Trading using Machine Learning

Tune the Baseline Trading Algorithm
In this section, you’ll tune, or adjust, the model’s input features to find the parameters that result in the best trading outcomes. You’ll choose the best by comparing the cumulative products of the strategy returns.

**Step 1: Tune the training algorithm by adjusting the size of the training dataset.**
To do so, slice your data into different periods. Rerun the notebook with the updated parameters, and record the results in your README.md file.

Answer the following question: What impact resulted from increasing or decreasing the training window?

We can see now that the impact on the trading window leads to higher actual results specifically from 2017-2018 onward as demonstrated by the figure here in comparison to the original actual results graph.

**Step 2: Tune the trading algorithm by adjusting the SMA input features.**
Adjust one or both of the windows for the algorithm. Rerun the notebook with the updated parameters, and record the results in your README.md file.

Answer the following question: What impact resulted from increasing or decreasing either or both of the SMA windows?

By increasing or decreasing the SMA window we get a either a more or less accurate representation of the data as by increasing the window we capture more of the data where as when we decrease the window it allows us to capture the data for a smaller period of time making it less accurate.

**Step 3: Choose the set of parameters that best improved the trading algorithm returns.**
Save a PNG image of the cumulative product of the actual returns vs. the strategy returns, and document your conclusion in your README.md file.

What we can see from the charts is that the biggest difference was made in the initial tuning of the baseline algorithm as we can see the actual returns inreased as as per the images above. Adding the logistic regression model did not make a difference as we can see by the two charts depicting the strategy returns vs the actual returns. The set of parameters that best improved the algorithms returns was adjusting the SMA windows. This makes sense as we increase the SMA windows we get a more and more accurate understanding of the long term behaviour and then that gives a better benchmark to compare our shorter moving window average too allowing for better decision making in our algorithm.


**Updated using 30 short window SMA and 400 long window SMA 3 month ending window remains the same**

![blob2](https://user-images.githubusercontent.com/117589787/224198256-3ab7067f-7d3e-4ef3-a0a7-0c08a6cf8e4f.jpg)

**Updated using 6 month ending window SMA remains same**

![blob2](https://user-images.githubusercontent.com/117589787/224198256-3ab7067f-7d3e-4ef3-a0a7-0c08a6cf8e4f.jpg)


**changing SMA to 30 and 400 and ending window to 6 month**

![blob3 original](https://user-images.githubusercontent.com/117589787/224199772-38ed89c7-f1f7-499e-b9d9-ce1cf13b6df0.jpg)

**original output short window 4, long window 100, ending 3 months**

![blob4](https://user-images.githubusercontent.com/117589787/224200140-94849666-1dbd-4662-b50b-d0a7f0cd4453.jpg)

**Logistic Regression Output**

![blob4](https://user-images.githubusercontent.com/117589787/224200140-94849666-1dbd-4662-b50b-d0a7f0cd4453.jpg)

What we can see that is that changing and the SMA and/or the month ending cut off as shown in the graphs above gives us a higher actual return showing the height of the graph at 1.8 as opposed to 1.4 from original benchmarked algorithm. 

When we include the logistic regression model we also dont see as much of an increase in the returns, only by adjusting the cut off end date and the SMA windows do we see the biggest changes
