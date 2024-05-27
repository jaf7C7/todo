# Solution

> Your task is to:
> * Analyze the relevant classes for the app and the attributes and methods of each class.
> * List the relevant attributes (and, if possible, the potential values) and write a brief description of the functionality of the methods.


## Possible classes and their attributes

* `Student`:
    * `todo_list list[Todo]`: A list of tasks the student must complete.
    * `university_courses list[Course]`: A list of university courses that the student is taking.
    * `create_todo(description, due_date, priority, type) -> None`: Create a new task and add it to the task list.
    * `mark_complete(todo Todo) -> None`: Completed to-dos are removed from the list.

* `Todo`:
    * `description str`: A string describing the task.
    * `due_date datetime.date`: The date of the task deadline.
    * `priority str`: One of `['Urgent', 'Intermediate', 'Optional']`.
    * `type str`: One of `['Personal', 'Academic', 'Work', 'Leisure']`.
    * `classroom str`: Default `None`, only used with `type='Academic'`.
    * `course Course`: See `classroom`.

* `Course`:
    * `code str`: Course ID code`
    * `professor str`: The professor teaching the course.
    * `start_time datetime.datetime`: The course start (time|date)?
    * `end_time datetime.datetime`: See above.
    * `classroom str`: The ID of the hosting classroom.