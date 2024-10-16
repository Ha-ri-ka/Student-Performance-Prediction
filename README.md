**DATASET** : https://www.kaggle.com/datasets/aljarah/xAPI-Edu-Data<br>
This is an educational data set that is collected from a learning management system (LMS) called Kalboard 360. The dataset consists of 480 student records and 16 features. The features are classified into three major categories:<br>
&nbsp;&nbsp;&nbsp;&nbsp;<i>(1) Demographic features such as gender and nationality.</i><br>
&nbsp;&nbsp;&nbsp;&nbsp;<i>(2) Academic background features such as educational stage, grade Level and section.</i><br>
&nbsp;&nbsp;&nbsp;&nbsp;<i>(3) Behavioral features such as raised hand on class, opening resources, answering survey by parents, and school satisfaction.</i><br>
The data contains students from 14 different countries. The target variable is a class that each student belongs to based on their academic performance: <br>
&nbsp;&nbsp;&nbsp;&nbsp;<i>Low-Level: interval includes values from 0 to 69</i><br>
&nbsp;&nbsp;&nbsp;&nbsp;<i>Middle-Level: interval includes values from 70 to 89</i><br>
&nbsp;&nbsp;&nbsp;&nbsp;<i>High-Level: interval includes values from 90-100</i><br>

**ANALYSIS,EXPLORATION AND VISUALIZATION OF DATA**<br>
Bar graph of marks scored versus subjects to identify the easiest and most difficult subjects.<br><br>
Bar graph of marks scored by students based on attendance, showing that higher attendance correlates with higher grades.<br><br>
Analyzing the relationship between resource visits and grades: no students fall into the LOW category if they access resources at least 80 times (scatter plot).<br><br>
Examining the relationship between discussion participation and grades: more discussions lead to better grades (scatter plot).<br><br>
The relationship between hand-raising frequency and grades: students with medium grades raise their hands the most, while high achievers participate the least, indicating medium performers rely more on class participation. Low-grade students show moderate participation.<br><br>
Students from lybia and kuwait have the most number of students scoring low marks amongst their peers from the same country, while students from Venezuela,Iraq and Saudi Arabia have the highest.<br><br>
There are identical low score ratios across all sections, suggesting that the section itself does not make a difference.<br><br>

Based on analysis, the columns that effect the final grade most:<br>
'raisedhands','VisITedResources','AnnouncementsView','Discussion','ParentAnsweringSurvey','StudentAbsenceDays','ParentschoolSatisfaction','Class'<br>

**ALGORITHMS USED**<br>
[All metrics are Macro-averages]<br><br>
<i>1.Logistic regression </i><br>
Precision:0.79&nbsp;&nbsp;recall:0.82&nbsp;&nbsp;F1-score:0.80&nbsp;&nbsp;Accuracy:0.79 <br><br>
<i>2.Multiple Linear regression </i><br>
Precision:0.79&nbsp;&nbsp;recall:0.82&nbsp;&nbsp;F1-score:0.80&nbsp;&nbsp;Accuracy:0.79 <br><br>
<i>3.Polynomial regression </i><br>
DEGREE 2: Precision:0.79&nbsp;&nbsp;recall:0.82&nbsp;&nbsp;F1-score:0.80&nbsp;&nbsp;Accuracy:0.79 <br>
DEGREE 3: Precision:0.32&nbsp;&nbsp;recall:0.32&nbsp;&nbsp;F1-score:0.32&nbsp;&nbsp;Accuracy:0.60 <br>
DEGREE 4: Precision:0.25&nbsp;&nbsp;recall:0.23&nbsp;&nbsp;F1-score:0.24&nbsp;&nbsp;Accuracy:0.58 <br><br>
<i>4.SVM </i><br>
accuracy<br>
LINEAR: 0.79 <br>
SIGMOID: 0.29 <br>
RBBF: 0.76 <br><br>
<i>5.Decision tree classifier </i><br>
MSE:0.28125&nbsp;&nbsp;Accuracy:0.71 <br><br>
