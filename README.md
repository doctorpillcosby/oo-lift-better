# LyftBetter™ 

## Deliverables
You're building a new fitness tracker app:
- your models are user, exercise, and log
  - a user has many logs
  - an exercise has many logs
  - a log belongs to an exercise and a user

Write out the relationships using has_many, belongs_to and has_many_through. Create the necessary methods to connect these classes.

#### User
- a user is initialized with a name

- `#logs`
  - returns all logs belonging to that user
- `#exercises`
  - returns all unique exercises performed by the user.
- `.all`
  - returns an array of all users

- `#log_exercise(exercise, weight, reps)`

- `#get_exercise_info(exercise)`
  - returns an array of logs for the specified exercise for the user

#### Exercise
- `#user`
  - returns all unique users who performed this exercise
- `#logs`
  - returns all logs this exercise is part of
- `.all`
  - returns an array of all drivers
- `#average_weight`
  - returns the average weight for lifted for this exercise
- `#strongest_lifter`
  - returns the user who lifted the heaviest weight for this exercise


#### Log
- a log is initialized with (exercise, weight, reps, user)
- `#user`
  - returns the user object for this log
- `#exercise`
  - returns the exercise object for this log
