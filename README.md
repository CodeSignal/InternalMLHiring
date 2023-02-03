# Requirements

You are given a jupyter notebook (`ipynb` file), containing models for scoring the code quality using proxy metrics, which are listed and described below. Your task is to fix problems in the notebook to make the model better. Most of the problems are associated with data preprocessing and model training.

## Feature explanation

* MAX_CYCLOMATIC - the maximum cyclomatic complexity of the functions in the code
* MEAN_CYCLOMATIC - the mean cyclomatic complexity of the functions in the code
* MEDIAN_CYCLOMATIC - the median cyclomatic complexity of the functions in the code

**Note:** cyclomatic complexity is a metric that measures the complexity of the code by the number of conditions and loops in it.

---

* MAX_COGNITIVE - the maximum cognitive complexity of the functions in the code
* MEAN_COGNITIVE - the mean cognitive complexity of the functions in the code
* MEDIAN_COGNITIVE - the median cognitive complexity of the functions in the code

**Note:** cognitive complexity is a measure of how difficult a unit of code is to intuitively understand. Unlike cyclomatic complexity, which determines how difficult your code will be to test, cognitive complexity tells you how difficult your code will be to read and understand.

---

* LENGTH - the length of the code in lines
* CALCULATED_LENGTH, VOLUME, DIFFICULTY, MAINTAINABILITY, EFFORT, TIME, BUGS - theoretical metrics estimated by the Halstead complexity model.

**Note:** Halstead complexity measures are used to estimate the effort required to develop, maintain, and modify a program. The Halstead complexity measures are based on the number of distinct operators and operands in a program.

---

* REVIEWER_1 - the code quality score evaluated by the first reviewer.
* REVIEWER_2 - the code quality score evaluated by the first reviewer.

**Note 1:** the reviewers were asked to score the code quality on a scale from 1 to 5, where 1 is the worst and 5 is the best, which was then converted to a scale from 0 to 1, where 0 is the worst and 1 is the best.

**Note 2:** there were 8 reviewers, but the code samples were split between them in a way that each sample was scored by 2 reviewers. The scores provided by each reviewer were scaled to have the same std and mean for each reviewer.
