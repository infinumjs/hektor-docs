# clean

## Implementation status

### Gulp: Implemented
### Grunt: None

## Options

  * deps
    * array of dependencies that should be loaded
    * default: ``[]``
  * before
    * tasks that will be executed before this task
    * gulp: tasks will be executed in parallel, but all of them are guaranteed to be done before this task is started
    * default: ``[]``
  * task
    * function that will be called when the task is called
    * default: ``function() {}``
    * receives three arguments
      * H - HEKTOR instance (contains deps, tasks and config)
      * options - options defined for the task in the grunt/gulp file (with parsed templates)
      * done - callback function (called with one argument - error)

# Async tasks (Gulp)
If a task is asyncronous it should do one of three things:
* Return a promise
* Return a stream
* Call the callback function
