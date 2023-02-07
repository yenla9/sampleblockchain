# Homework #14: Machine Learning Trading Bot
### By: Yen

### Establish a Baseline Performance
Write your conclusions about the performance of the baseline trading algorithm in the `README.md` file that’s associated with your GitHub repository. Support your findings by using the PNG image that you saved in the previous step.

![Baseline](./Image/baseline.PNG)
![baseline_report](./Image/report_svc.PNG)

Based on the SVC classifier model, the precision for selling stock is 100%, while buying stock is 63%. When selling it is at 6% positive and when buying it is 100% positive.  Overall, the Strategy Returns is higher than Actual Returns.

### Tune the Baseline Trading Algorithm
1. Tune the training algorithm by adjusting the size of the training dataset. To do so, slice your data into different periods. Rerun the notebook with the updated parameters, and record the results in your `README.md` file. Answer the following question: What impact resulted from increasing or decreasing the training window?
![6Months](./Image/6months_dateoffset.PNG)
![6Months](./Image/report_6monthsoffset.PNG)

    When I changed the DateOffset to 6 months, the selling stock precision dropped from 100% to 59%, while buying stock precision went down from 63% to 58%. The recall for selling stock went from 6% to 20% positive and buying stock went down from 100% to 89% positive. 

2. Tune the trading algorithm by adjusting the SMA input features. Adjust one or both of the windows for the algorithm. Rerun the notebook with the updated parameters, and record the results in your `README.md` file. Answer the following question: What impact resulted from increasing or decreasing either or both of the SMA windows?

    ![50Long](./Image/long_50_graph.PNG)
    ![50_report](./Image/long_50.PNG)

    When the long window changed from 100 to 50, the precision for selling stock stays the same but the precision of buying stock went up 4% and the recall for selling is 7% instead of 6% positive.

3. Choose the set of parameters that best improved the trading algorithm returns. Save a PNG image of the cumulative product of the actual returns vs. the strategy returns, and document your conclusion in your `README.md` file.

    ![item3](./Image/item3.PNG)
    ![report_item3](./Image/report_item3.PNG)
    
    When I changed the short window = 10 and DateOffSet = 4 months, there is higher yield of positive when selling the stocks but the precision went down for selling the stocks. 

### Evaluate a New Machine Learning Classifier
Backtest the new model to evaluate its performance. Save a PNG image of the cumulative product of the actual returns vs. the strategy returns for this updated trading algorithm, and write your conclusions in your `README.md` file. Answer the following questions: Did this new model perform better or worse than the provided baseline model? Did this new model perform better or worse than your tuned trading algorithm?

### Baseline
![Baseline](./Image/baseline.PNG)
![baseline_report](./Image/report_svc.PNG)
### Decision Tree
![Decision](./Image/decisiontree.PNG)
![Decision_report](./Image/report_decision.PNG)
### Ada Boost
![Ada](./Image/adaboost.PNG)
![Ada_report](./Image/report_ada.PNG)
### Logistic Regression 
![Log](./Image/Logistic.PNG)
![Log_report](./Image/report_log.PNG)

The Decision Tree performs better than the baseline, Ada Boost and Logistic Regression models. 

### Evaluation Report
 For this report, express your final conclusions and analysis. Support your findings by using the PNG images that you created.

Depending on the data set, using the right Machine Learning Classifier will be important. As I was testing different models, Decision Tree classifier yielded better results than the other models. Therefore, it is important to test out different classifier to see which one is better for the data set. 

![Decision](./Image/decisiontree.PNG)
![Decision_report](./Image/report_decision.PNG)



