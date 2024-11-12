# Introduction to ML

## What is Machine Learning?

* __Tom M\. Mitchell \(1997\)__ :
  * "A computer program is said to learn from experience  _E_  with respect to some class of tasks  _T_  and performance measure  _P_ \, if its performance at tasks in  _T_ \, as measured by  _P_ \, improves with experience  _E_ \."
  * Source:  _Machine Learning_ \, Tom M\. Mitchell\, McGraw Hill\, 1997\.
* __Arthur Samuel \(1959\)__ :
  * "Machine Learning is the subfield of computer science that gives computers the ability to learn without being explicitly programmed\."
  * Arthur Samuel is credited with coining the term "Machine Learning" in 1959\. He's known for his work on the Samuel Checkers\-playing Program\.
* __Kevin P\. Murphy \(2012\)__ :
  * "Machine learning is a set of methods that can automatically detect patterns in data\, and then use the uncovered patterns to predict future data\, or to perform other kinds of decision\-making under uncertainty \(such as planning how to collect more data\)\."
  * Source:  _Machine Learning: A Probabilistic Perspective_ \, Kevin P\. Murphy\, MIT Press\, 2012\.
* __Aurélien Géron \(2015\)__ :
  * "Machine Learning is the science \(and art\) of programming computers so they can learn from data\.”
  * Source: Hands\-on Machine Learning \(your text\-book\!\)

## ML Origins

* __Early Theoretical Foundations__ :
  * “Reason\.\.\. is nothing but Reckoning \(that is\, Adding and Subtracting\) of the Consequences of general names agreed upon for the marking and signifying of our thoughts\.\.\.” –  _Thomas Hobbs\, Leviathon \(1651\)_
* __Turing Test \(1950\)__ :
  * A "universal machine" that could simulate the behavior of any other machine
  * The "Turing Test" as a measure of a machine's ability to exhibit intelligent behavior indistinguishable from that of a human\.
* __Advent of Electronic Computers \(1940s\-1950s\)__ :
  * The creation of electronic computers provided the necessary tools for exploring computational approaches to problem\-solving\.
* __Birth of Artificial Intelligence \(1956\)__ :
  * At the Dartmouth Workshop in 1956\, the term "Artificial Intelligence" \(AI\) was coined\. This event is often considered the birth of AI as a formal academic discipline\. Early AI research focused on problem\-solving\, logical reasoning\, and symbolic methods\.

![](assets/IST707-Week10.jpg)

# Applications of Machine Learning

* __Healthcare & Life Sciences__
  * Disease Identification & Diagnostics\,  Drug Discovery & Personalized Medicine\, Predictive Analytics
* __Finance & Banking__
  * Fraud Detection\,  Algorithmic Trading\,  Credit Scoring
* __E\-Commerce & Retail__
  * Recommendation Systems\, Demand Forecasting\, Customer Sentiment Analysis
* __Automotive & Transportation__
  * Autonomous Vehicles\,  Predictive Maintenance\, Traffic Prediction
* __Energy & Utilities__
  * Smart Grid Management\, Predictive Maintenance for Equipment\, Energy Consumption Forecasting
* __Entertainment & Media__
  * Content Recommendation\, Sentiment Analysis\, Automated Content Creation

# The Importance of Communication

* __Translating Technicalities__ :
  * ML involves intricate algorithms\, complex mathematical models\, and vast amounts of data\.
  * Stakeholders are often more interested in the  _actionable insights\._
  * ML practitioners must articulate findings in a comprehensible and meaningful manner\.
* __Understanding Stakeholder Needs__
  * Essential to understand the problem from a stakeholder's perspective\. Aims? Constraints?
  * Solutions must meet the needs of those who will use or be affected by the model\.
* __Setting Clear Expectations__ :
  * Overhype leads to disappointment and mistrust\.
  * Misuse can cause substantive harm
  * Vital to communicate what a model can and cannot do\, its limitations\, and any uncertainties involved\.
* __Ethical Considerations__ :
  * Increasing concerns about ML’s ethical implications\, potential biases\, and fairness\.
  * Transparent communication about how models work and their potential pitfalls is crucial\.

# Failures of Communication

* __Google Flu Trends__  <span style="color:#D1D5DB">: </span>
  * Google’s attempt to predict flu outbreaks using search query data\.
  * High expectations and inconsistent performance led to skepticism about the utility of big data
  * Effort terminated\.
* __IBM Watson for Oncology__  <span style="color:#D1D5DB">:</span>
  * Promised to revolutionize cancer treatment by providing personalized treatment recommendations
  * Erroneous treatment recommendations & over\-promotion of Watson's capabilities without clear communication about its limitations
  * Effort terminated

# The Case of COMPAS

* __COMPAS \(Correctional Offender Management Profiling for Alternative Sanctions\)__
  * Risk assessment tool used by the U\.S\. courts to assess the likelihood of recidivism
* __Fairness and Goal alignment__
  * ProPublica Analysis \(2016\): Black defendants had high false positive rate\, white defendants had high false negative rate
  * Northpointe Rebuttal: “Predictive parity\.” Risk levels equivalent across groups
* __Misuse__
  * Designed to aid in decisions about pretrial release\, parole\, and probation
  * But documented cases of being used for sentencing guidelines
* __Transparency Issues__
  * proprietary tool; inner workings are not open to public scrutiny
  * ethical questions about the use of "black\-box" models in consequential decisions

# Introduction to the Python ML Ecosystem
Machine Learning in Python is characterized by an ecosystem of libraries, each specializing in different aspects of the ML workflow. This ecosystem simplifies the process of developing and implementing ML models and ensures efficiency and versatility. The integration between these libraries allows for a streamlined workflow, from initial data handling to final model deployment.

There are many many online resources for learning to use these libraries, and chatbots like ChatGPT are generally quite fluent with this ecosystem. I have included several pointers to get you started for each of the following, but this is just the tip of a much larger iceberg.

### 1. Python
Python is a high level programming language with a straightforward syntax that helps programmers develop highly readable code. Python is the foundation upon which the following libraries are built, offering a unified scripting environment.

**Resources**
- **Official Python Documentation**: [docs.python.org](https://docs.python.org)
- **Python Tutorial by Python.org**: [Python.org Tutorial](https://docs.python.org/3/tutorial/)
- **Real Python**: Offers tutorials and articles on various Python topics - [Real Python](https://realpython.com/)

### 2. Pandas
Pandas is typically the starting point in the data science workflow. Provides DataFrame for efficient storage and manipulation of tabular data, and incorporates tools for handling missing data, merging, reshaping, and slicing datasets. It's used for:
- **Data Import and Wrangling**: Reading data from various sources and performing initial transformations.
- **Data Analysis**: Simplifies exploratory data analysis with built-in functions.
- **Interfacing with Other Libraries**: Pandas integrates well with libraries like Numpy for numerical operations, Matplotlib and Seaborn for visualization, and can feed data directly into machine learning models in Scikit-Learn.

**Resources**
- **Official Documentation**: [pandas.pydata.org](https://pandas.pydata.org/docs/)
- **Pandas Getting Started Tutorials**: [Pandas Tutorials](https://pandas.pydata.org/docs/getting_started/index.html#getting-started)
- **Kaggle Pandas Course**: [Kaggle Pandas](https://www.kaggle.com/learn/pandas)

### 3. Numpy
Numpy excels in numerical computations. It provides efficient operations with arrays and matrices, thanks to its implementation in C. Numpy supports a wide range of mathematical operations, which is fundamental in ML for data manipulation and transformation. Numpy is:
- **A Backbone for Pandas and Scikit-Learn**: Many Pandas operations are built on Numpy, and Scikit-Learn utilizes Numpy arrays for optimal performance in model training and predictions.
- **Essential for Numerical Analysis**: Any heavy numerical computation, especially involving arrays and matrices, relies on Numpy for efficiency.

**Resources**
- **Official Documentation**: [numpy.org/doc](https://numpy.org/doc/stable/)
- **Numpy User Guide**: [Numpy User Guide](https://numpy.org/doc/stable/user/index.html)
- **SciPy Lectures on Numpy**: [SciPy Lectures](http://scipy-lectures.org/intro/numpy/index.html)

### 4. Matplotlib and Seaborn
Visualization is essential for understanding data distributions, patterns, and insights, and hence indispensible in ML for data exploration and analysis of results. These libraries are the most widely used visualization tools in the ML ecosystem, and directly use Pandas data structures for plotting; Numpy's numerical capabilities augment plotting functionalities   
- **Matplotlib**: A versatile library for creating a wide range of static, animated, and interactive plots.
- **Seaborn**: Built on top of Matplotlib, it provides a high-level interface for drawing attractive and informative statistical graphics, making complex visualizations more accessible.

**Resources**

Matplotlib:
- **Official Documentation**: [matplotlib.org](https://matplotlib.org/stable/contents.html)
- **Matplotlib Tutorials**: [Matplotlib Tutorials](https://matplotlib.org/stable/tutorials/index.html)
- **Python Graph Gallery**: [Python Graph Gallery](https://www.python-graph-gallery.com/matplotlib)

Seaborn:
- **Official Documentation**: [seaborn.pydata.org](https://seaborn.pydata.org/)
- **Seaborn Tutorial**: [Seaborn Tutorial](https://seaborn.pydata.org/tutorial.html)
- **DataCamp Seaborn Tutorial**: [DataCamp Seaborn](https://www.datacamp.com/community/tutorials/seaborn-python-tutorial)


### 5. Scikit-Learn
Scikit-Learn is where the ML models come to life. It provides a wide array of supervised and unsupervised learning algorithms, as well as tools for feature selection, normalization, and cross-validation. While scikit-learn can use Pandas data frames directly, Scikit-Learn is optimized for Numpy arrays. It is therefore important to understand data conversion and manipulation across these libraries.

**Resources**
- **Official Documentation**: [scikit-learn.org](https://scikit-learn.org/stable/documentation.html)
- **Scikit-Learn User Guide**: [Scikit-Learn User Guide](https://scikit-learn.org/stable/user_guide.html)
- **Scikit-Learn Tutorials**: [Scikit-Learn Tutorials](https://scikit-learn.org/stable/tutorial/index.html)

### Conclusion
In this ecosystem, each library has a distinct role but is also intricately connected with the others. Pandas and Numpy handle the data preparation; Matplotlib and Seaborn assist in data visualization; and Scikit-Learn is used for building and evaluating machine learning models. Understanding how to navigate these libraries and leverage their interconnectedness is crucial for any aspiring data scientist or ML practitioner. 