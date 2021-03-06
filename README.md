# Weather Scheduler

An automated solution for scheduling events based on the weather forecast.

The weather scheduler program gets weather information for a specific location,
date and time. The weather data can be used in event templates that can be
emailed to a group of people.

## Problem
The local bicycle club has weekly rides on Monday and Wednesday nights. Each
day before the ride someone looks up the wind direction, wind speed,
temperature and sunset time to schedule the rides. Scheduling the weekly group
rides is a manual task that takes a human time to complete each week.

## Solution
Create an automated script that can gather the on-line weather information,
create the event text and email the information out to a group.

## Information

**Requirements**: Must be easier to use than performing the tasks manually.

**Budget**: Zero dollars.

Read the [DESIGN.md](DESIGN.md) document for more details and
phases of the application development.

Read the [RESEARCH.md](RESEARCH.md) document for links, references,
and information on the technologies used in the application.

# Usage

The program can be run on the command line without any flags and will prompt
the user for the options.

```
weather_scheduler/weather_scheduler.py
```

If you know the options you want you can call the program with the flags.

```
weather_scheduler/weather_scheduler.py --day monday --time '6:00 PM' --key WU_KEY --location MN/Rochester --context "comment=It is getting dark fast so bring a light.,footer=Ride safe."

weather_scheduler/weather_scheduler.py --day wednesday --time '6:00 PM' --key WU_KEY --location MN/Rochester --context "comment=It is getting dark fast so bring a light.,footer=Ride safe."
```
