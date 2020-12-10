# dateable

SQL does not support generating data in a range. For instance, one can use "Select x from table_y where x between a and b;", but one cannot do something like the following: "Select x from a to b". This project was aimed at addressing that specific shortcoming, as relates to date values. I have not yet needed to generate a range of specific time-values (such as hourly appointment slots), so it only reflects the need I experienced, being for specific days contained by a range, that range being year 2005 to year 2100.

Using this project, one may perform the following: "Select value from dateable.reference_possible_date_values where value between '2009-10-01' and '2009-11-01'", and can expect each distinct date value having time component "00:00:00", October 1st 2009 to November 1st 2009.
