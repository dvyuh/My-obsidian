
**Controllers** are where you write the actual business logic for your routes. They contain the functions that talk to the database (using Mongoose) and send responses back to the user.

```
const getWorkouts = async (req, res) => {

const workouts = await Workout.find({}).sort({createdAt: -1})

res.status(200).json(workouts)
}
```

this example code is the controller for getting all the available workouts.

first creating a function getworkouts. -> * it is an async function * because it is requesting the data from the servers. 
-> **next it searches all the workout using the find tag.**
and sorts them wrt the time it was created

---
