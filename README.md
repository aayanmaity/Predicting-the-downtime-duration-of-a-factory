# Predicting-the-downtime-duration-of-a-factory

Identifying factories that are most prone to downtime by predicting downtime duration of various factories,
using 6 different datasets, determining important features with Chi-squared test, handled high cardinal categorical variable with
target encoding and used cross-validation to avoid overfitting and built multiclass classification machine learning model.




## Project Details:

An electric car manufacturing company, 'Kesla', with several factories is seeing exponential growth in
demand due to the sudden increase of subsidies for EVs in the country.

The car manufacturer, however, is not able to handle the demand and has tasked a team of Data
Science consultants to identify potential areas to quickly increase the efficiency without operational
changes.

The team of Data Science consultants saw that without changing any of the data that is being collected, a predictive model can be built that predicts the downtime of a factory, thereby allowing the few engineers present in the engineering team to very quickly most important factories that would cause the most significant downtime.

The Chief Data Scientists have now curated a
dataset, where we have several variables that it
believes impact the `downtime_duration`. They have tracked three different downtime durations.

The three classes of `downtime_duration`
* `0` - Low downtime (15 minutes to 1 hour).
* `1` - Downtime that lasts anywhere between 1 hour and 24 hours.
* `2` - for long downtimes that can last from 24 hours to sometimes even several days.

We will now have to use this curated data to create a machine learning model that will be able to
predict the `downtime_duration` so that the company can better handle downtimes and increase
operational efficiency to better handle demand.

# Dataset Description:

Target attribute: "downtime_duration" (discrete_variable: 3 classes)

There are 6 CSV files provided to us, they are described below:

* `train_data.csv`: It has a unique event id for each observation of the downtime_duration in
a particular factory_number
* `test_data.csv`: Similar to the train dataset, we are provided with an id and a
factory_number, we are expected to predict the outage_duration for each of the records
* `assembly_line_info.csv`: For each of the event ids mentioned in the train_data.csv and
test_data.csv files and also some additional ids there is a record of the
assembly_line_type that is stored in the dataset. There are 10 different types of assembly
lines that are observed in the dataset. There can be multiple assembly lines in a single
factory, for the factory to be running all the assembly lines must be functioning.
* `issue_info.csv`: For each of the event ids mentioned in the train_data.csv and
test_data.csv files and also some additional ids there is a record of the issue_type that is
stored in the dataset. There are 5 different issue_type's recorded in the dataset. These
are classified as an issue by an onsite engineer.
* `log_report_type_data.csv`: For each event id there are log_report_type and volume
columns are recorded. log_report_type is a type of the recorded report as reported by a
technical team member who is working on the assembly line. Workers are allowed to
report specific types of issues using a mobile application. volume is the volume of cars
handled by the assembly line in custom company specific units.
* `car_variant_data.csv`: For each of the event ids mentioned in the train_data.csv and
test_data.csv files and also some additional ids there is a record of the car_variant_type
that is being put together on the assembly line.


# Tools used:

**Code**: Python Version: 3.7

**For data wrangling and visualization**: NumPy, Pandas, Matplotlib, Seaborn

**For predictive analytics**: SciPy, scikit-learn, LightGBM, Tensorflow, Keras

**For Reporting**: Canva

