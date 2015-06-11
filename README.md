# MySQL and Highcharts Reactive Leaderboard Example

The familiar Meteor Leaderboard example modified to use a MySQL backend as well as a Highcharts, reactively!

This example uses the following packages 

For MySQL integration: 
* [numtel:mysql](https://github.com/numtel/meteor-mysql)

For Highcharts integration:
* [maazalik:highcharts] (https://github.com/MaazAli/Meteor-HighCharts)

## Quick start

This example requires a MySQL server configured to output the binary log in row mode.

See [the `mysql-live-select` installation instructions](https://github.com/numtel/mysql-live-select#installation) for more details...

```bash
$ git clone https://github.com/numtel/meteor-mysql-leaderboard.git
$ cd meteor-mysql-leaderboard

# Create new database
$ mysql -uUSERNAME -pPASSWORD -e "create database leaderboard"

# Import sample tables and data
$ mysql -uUSERNAME -pPASSWORD DATABASE < leaderboard.sql

# Update database connection settings in your favorite editor
$ ed leaderboard.js

$ meteor
```

## Highcharts integration

For this example I have just added a pie chart using Highcharts. For convenience and demonstration I have used the [maazalik:highcharts] (https://github.com/MaazAli/Meteor-HighCharts) package. 
Of course the same can be achieved without thi package using a little jQuery.

The demo demonstrates nicely how the pie chart reactively changes in line with updates to the MySQL database.   

## License Highcharts

Highcharts is free for personal and non-profit projects. For other purposes click [here](http://shop.highsoft.com/highcharts.html).