# In this tutorial, you will learn about date and time in JavaScript with the help of examples.

In JavaScript, date and time are represented by the Date object. The Date object
provides the date and time information and also provides various methods.
A JavaScript date defines the EcmaScript epoch that represents milliseconds
since 1 January 1970 UTC. This date and time is the same as the UNIX epoch
(predominant base value for computer-recorded date and time values).

# Creating Date Object
 There are four ways to create a date object.
1 •new Date()
2 •new Date(milliseconds)
3 •new Date(Date string)
4 •new Date(year, month, day, hours, minutes, seconds, 
milliseconds

# 1-new Date()
You can create a date object using the new Date() constructor. For example,
// Create a new Date
const timeNow=new Date()
console.log(timeNow)

# 2-new Date(milliseconds)
A Date object contains a number representing milliseconds 
since January 1, 1970 UTC. New Date(milliseconds) Creates a 
new Date object by adding milliseconds to the zero time. For 
example
const timeNow=new Date(0)
console.log(timeNow)
// Chavobsh
Wed Dec 31 1969 16:00:00 GMT-0800 (Pacific Standard Time)

# 3-new Date (date string)
New Date - (date string) creates a new date object from the date string.In JavaScript, there 
are generally three date input formats. ISO Date Formats You can create a date object by 
passing ISO date formats. For example

const timeNow=new Date("2022")
console.log(timeNow)

# 4-new Date (year, month, day, hours, minutes, seconds, milliseconds)
new Date(year, month,...) creates a new date object with the specified date 
and time. For example

const timeNow=new Date(2006,08,03)
console.log(timeNow)

Note: If you pass only one argument, it will count as milliseconds. 
Therefore, to use this date format, you must pass two arguments. In 
JavaScript, months are counted from 0 to 11. January is 0 and 
December is 11


// Methods for date
# 1-now()
Date.now() returns the number of milliseconds since January 1, 1970

const timeNow= Date.now(2006,08,03)
console.log(timeNow)

# 2-getFullYear()
getFullYear() returns the full year of a date (4 digits)

const timeNow=new Date()
console.log(timeNow.getFullYear())

# 3-getMonth()
getMonth() returns the month (0 to 11) of the date. January = 0, February = 1, .

const timeNow=new Date()
console.log(timeNow.getMonth())

# 4-getDate()
The getDate() method returns the day of the month (1 to 31) of the date

const timeNow=new Date()
console.log(timeNow.getDate())

# 5-getDay()
The getDay() method returns the day of the week (0 to 6) of the date. Sunday = 0, Monday = 1

const timeNow=new Date()
console.log(timeNow.getDay())

# 6-getHours()
getHours() returns the hours (0 to 23) of a date.

const timeNow=new Date()
console.log(timeNow.getHours())


# 7-getMinutes
getMinutes() returns the minutes (0 to 59) of a date.

const timeNow=new Date()
console.log(timeNow.getMinutes())


# 8-getUTCDate()
getUTCDate() returns the day of the month (1 to 31) of a date object. 
getUTCDate() returns the date in UTC.

const timeNow=new Date()
console.log(timeNow.getUTCDate())


# setFullYear()
setFullYear() sets the year of the date.
setFullYear() can also set the month and day


const timeNow=new Date()
let b=timeNow.setFullYear("2023")
console.log(timeNow)


# setMonth()
The setMonth() method sets the month of the date object.
This method can also be used to set the day of the month.


const timeNow=new Date()
let b=timeNow.setMonth("11")
console.log(timeNow)

# setUTCDate()


const timeNow=new Date()
let b=timeNow.setUTCDate("11")
console.log(timeNow)