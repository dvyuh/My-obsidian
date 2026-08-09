here this time i used mongodb atlas. 
a database that i can create and store online.
sometime later i'll try to understand offline

---

so here i installed mongoose
```
npm install mongoose
```


then connect using.
```
const mongoose = require('mongoose')
```


then connected to server 
```
mongoose.connect(process.env.MONGO_URI)

.then(() => {
//listen for requests
app.listen(process.env.PORT, () => {
console.log('connected to db & listening on port', process.env.PORT);
});})

.catch((error) => {
console.log(error);

})
```

MongoDB saves the data in a JSON formatt.

### Mongoose
Mongoose allows you to draw up a strict blueprint (called a **Schema**) for your data before it ever touches the database.

example code
```
const Schema = mongoose.Schema;

// 1. Create the Blueprint (Schema)
const workoutSchema = new Schema({
    title: {
        type: String,
        required: true
    },
    reps: {
        type: Number,
        required: true
    },
    load: {
        type: Number,
        required: true
    }
}, { timestamps: true }); // Automatically adds "createdAt" and "updatedAt" tags!

// 2. Wrap it in a Model and Export it
module.exports = mongoose.model('Workout', workoutSchema);
```

---

