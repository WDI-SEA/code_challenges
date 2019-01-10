# Calendar Fun 

## Historical Background

The [Gregorian Calendar](https://en.wikipedia.org/wiki/Gregorian_calendar), which is the calendar currently in use in most of the world, was introduced by Pope Gregory XII in 1582. The main feature is adding a leap year (which is a year with an extra day) roughly every 4 years. This helped account for the fact that the number of days in a year was an even number. In fact, the true amount of days in a year is about 365.2422. Thus, adding an extra day every 4 years helped account for that extra time, which had been causing the previous calendar, the Julian calendar to be offset from the actual seasons. Being the leader of the Christian church, Pope Gregory was worried that Easter would start happening in the summer.

![](https://upload.wikimedia.org/wikipedia/commons/5/52/Pope_Gregory_XIII_portrait.jpg)

The Gregorian calendar wasn't widely adopted until a couple centuries later when the British empire began to use it. Thus, the first practiced leap year was not until 1752. However, for the sake of our algorithm, we'll assume the calendar starts in the year 1582.

## Your Job

Given any valid date after 1582, print the day of the week it was. We'll complete this by breaking it down into 6 steps.

#### Test Cases

Use your birthday as your test case! After you get your birthday down, test some other dates, including dates like February 29th in leap years to make sure your algorithm works!

## Part 1: Leap Years

Write a function called `isLeapYear` that takes a year as an argument and returns `true` if the year was a leap year or will be a leap year. 

Note: Your function should work for future dates (e.g., 2028 should return true, 2029 should return false)

For past dates, previous to 1582, you can return true or false based on whether the year would have been a leap year if the calendar had been in use. You can assume that the year you are given is a valid year which is greater than or equal to 1582.

### Starter Code

#### JavaScript ES5 and below

```JavaScript
function isLeapYear(year){
    // Your code here
}
```

#### JavaScript ES6+

```JavaScript
const isLeapYear = (year) => {
    // Your code here
}
```

#### Python

```python
def is_leap_year(year):
    # Your code here
```

## Part 2: Count the Leaps

Now that you have a function that tells you whether a year is a leap year, use it as a helper function for this next portion. Write a function called `countLeapYears` that takes a start year and an end year and returns the number of leap years between the two. 

**Don't count the end year in the number of leap years.** For example, given the years 2016 and 2020, assume this time frame means 01/01/2016 through 12/31/2019. Thus the number of leap years ~~between~~ 2016 and 2020 is 1. Your function will determine that answer by checking the years 2016, 2017, 2018, and 2019.

```
2016: leap year
2017: not a leap year
2018: not a leap year
2019: not a leap year
```

> HINT: What if the user gives you the dates out of order? Make your function more agile by swapping the start and end year values if the user provides them out of order!

### Starter Code

#### JavaScript ES5 and below

```JavaScript
function countLeapYears(startYear, endYear){
    // Your code here
}
```

#### JavaScript ES6+

```JavaScript
const countLeapYears = (startYear, endYear) => {
    // Your code here
}
```

#### Python

```python
def count_leap_years(start_year, end_year):
    # Your code here
```

## Part 3: Count Days Between Years

Take your previous solution one step further and write a function called `countDaysInYears` that also takes two arguments of a start year and an end year. This should count the number of days between the two years (up to, but not including the end year). For example, `countDaysInYears(2019, 2020)` should return 365, because 2019 isn't a leap year.

As before, please handle the case where the user gives you the dates out of order!

### Starter Code

#### JavaScript ES5 and below

```JavaScript
function countDaysInYears(startYear, endYear){
    // Your code here
}
```

#### JavaScript ES6+

```JavaScript
const countDaysInYears = (startYear, endYear) => {
    // Your code here
}
```

#### Python

```python
def count_days_in_years(start_year, end_year):
    # Your code here
```

## Part 4: Find Days Year To Date

Given a valid date, determine the number of days that occured before that month. For example, given the date `September 11th, 1985`, determine the number of days that have passed within that year. You may wish to break this down into days in the current month (11) and days that have occurred in the months previous (from `January 1, 1985` to `August 31st, 1985`).

> HINT: Make sure to account for leap years!

### Starter Code

#### JavaScript ES5 and below

```JavaScript
function daysYearToDate(date){
    // Your code here
}
```

#### JavaScript ES6+

```JavaScript
const daysYearToDate = (date) => {
    // Your code here
}
```

#### Python

```python
def days_year_to_date(date):
    # Your code here
```

## Part 5: Find the Day of Week

Pick a year that starts on a Sunday to use as an anchor date. For example, 1589 is one you can use, but you can pick any one you'd like.

Write a function called `findDayOfWeek` that takes a number of days since your anchor date and calculate what day of the week it is using modulus 7, because there are always 7 days in a week, even between years.

> HINT: Use your other functions as helpers!

### Starter Code

#### JavaScript ES5 and below

```JavaScript
var ANCHOR_YEAR = 1589;

function dayOfWeek(date){
    // Your code here
}
```

#### JavaScript ES6+

```JavaScript
const ANCHOR_YEAR = 1589

const dayOfWeek = (date) => {
    // Your code here
}
```

#### Python

```python
ANCHOR_YEAR = 1589

def day_of_week(date):
    # Your code here
```

## Part 6 (BONUS): Pretty Printing

Write a function called `prettyPrint` that takes a date calls your previous functions in order to produce the given results:

#### Function Call

```
prettyPrint(new Date('09/11/1985'));
```

#### Results

> "The date 09/11/1985 was a Wednesday"

### Starter Code

#### JavaScript ES5 and below

```JavaScript
function prettyPrint(date){
    // Your code here
}
```

#### JavaScript ES6+

```JavaScript
const prettyPrint = (date) => {
    // Your code here
}
```

#### Python

```python
def pretty_print(date):
    # Your code here
```

## Answers

This is a work in progress! Eventually there will be a solutions branch with JavaScript and Python solutions for all problems and sub-problems. Until then, your instructor will go over the solution in the language of choice.

