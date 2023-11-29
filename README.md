# Answer of Assessment Hard Skill
>[!NOTE]
>this repo is just to store my answer from the assessment hard skill

## Level 1-2

### Structure Query Language (SQL) - Basic (HS)

1. Create the Students table.
```sql
CREATE TABLE Students (
    student_id INT PRIMARY KEY,
    first_name TEXT,
    last_name TEXT,
    age INT,
    grade TEXT
);
```

2. Retrieve All Student
```sql
SELECT * FROM Students;
```
---------- 
### Mobile Programming ( Android/IOS) - Basic (HS)
I choose React Native Framework to create Mobile Programming task due to the programming language that I've learned and I have experienced with it.

```javascript
// Import necessary components from React Native
import React from 'react';
import { View, Text, StyleSheet } from 'react-native';

// Create a functional component for the mobile app
const App = () => {
  return (
    <View style={styles.container}>
      <Text style={styles.text}>Hello, Mobile World!</Text>
    </View>
  );
};

// Define styles using StyleSheet
const styles = StyleSheet.create({
  container: {
    flex: 1,
    justifyContent: 'center',
    alignItems: 'center',
    backgroundColor: '#f0f0f0',
  },
  text: {
    fontSize: 24,
    fontWeight: 'bold',
    color: '#333',
  },
});

// Export the App component as the entry point of the application
export default App;

```

To execute this code and run the app:

- Set up development environment by installing Node.js, npm, and React Native CLI.
- Create a new React Native project using the `react-native init MyApp` command in terminal.
- Replace the default contents of the `App.js` or `index.js` file in the newly created React Native project with the code provided above.
- Run the application on a simulator/emulator or a physical device using the appropriate command (`react-native run-android` for **Android** or `react-native run-ios` for **iOS**).

-----------

### Frontend Programming (Html/ CSS/Bootstrap/CI) - Basic (HS)
```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>My Web Page</title>
</head>

<body>
    <h1>Welcome to My Web Page</h1>
</body>

</html>
```
