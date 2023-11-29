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
import React from 'react';
import { View, Text, StyleSheet } from 'react-native';

const App = () => {
  return (
    <View style={styles.container}>
      <Text style={styles.text}>Hello, Mobile World!</Text>
    </View>
  );
};

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

---------

### Back-end Programming (PHP/ C#/C++/Dart) - Basic (HS)

1. Node.js server

```node

const express = require('express');

const app = express();

app.get('/hello', (req, res) => {
  res.json({ message: 'Hello, World!' });
});

const PORT = 3000;
app.listen(PORT, () => {
  console.log(`Server is running on port ${PORT}`);
});

```
2. SQL

```sql
SELECT * FROM users;
```

## Level 3

### Structure Query Language (SQL) - Intermediate / Internal Training (HS)

1. Subquery

```sql
SELECT c.name AS customer_name, o.order_date
FROM Customers c
INNER JOIN Orders o ON c.customer_id = o.customer_id
WHERE o.quantity > (
    SELECT AVG(quantity) 
    FROM Orders
)

```
the result would look like this:
| customer_name | order_date |
|-------------- | ---------- |
| John Doe      | 2023-01-10 |

2. JOIN Operation

```sql
SELECT c.name AS customer_name, o.product
FROM Customers c
JOIN Orders o ON c.customer_id = o.customer_id;

```

the result would look like this:
| customer_name | product |
| ------------- | ------- |
| John Doe      | Laptop  |
| Jane Smith    | Smartphone |
| John Doe | Tablet |

-----

### Data Visualization using Business Intelligence (Fine Bi or Other) - Intermediate / Internal Training (HS)
 
 FineBI

-------
 
### Mobile Programming ( Android/ IOS) - Intermediate / Internal Training (HS)

```javascript
import React from 'react';
import { StyleSheet, Text, View } from 'react-native';

export default function App() {
  return (
    <View style={styles.container}>
      <Text style={styles.text}>Hello, Android!</Text>
    </View>
  );
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    justifyContent: 'center',
    alignItems: 'center',
    backgroundColor: '#fff',
  },
  text: {
    fontSize: 24,
    fontWeight: 'bold',
    color: '#333',
  },
});

```

---------

### Frontend Programming (Html/ CSS/ Bootstrap/ CI) - Intermediate/ Internal Training (HS)

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>My Personal Profile - AdiSite</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        .contact-form {
            width: 300px;
            margin: 20px auto;
            padding: 20px;
            border: 1px solid #ccc;
            border-radius: 5px;
            background-color: #f9f9f9;
        }
        
        .form-group {
            margin-bottom: 15px;
        }
        
        label {
            display: block;
            margin-bottom: 5px;
            font-weight: bold;
        }
        
        input[type="text"],
        input[type="email"],
        textarea {
            width: 100%;
            padding: 8px;
            border: 1px solid #ccc;
            border-radius: 3px;
            font-size: 14px;
        }
                
        button[type="submit"] {
            width: 100%;
            padding: 10px;
            border: none;
            border-radius: 3px;
            background-color: #007bff;
            color: #fff;
            font-size: 16px;
            cursor: pointer;
        }
        
        button[type="submit"]:hover {
            background-color: #0056b3;
        }
    </style>

</head>

<body>
    <h1>Personal Profile:</h1>

    <form action="#" method="post" class="contact-form">
        <div class="form-group">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" placeholder="ex: adi g" required>
        </div>

        <div class="form-group">
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" placeholder="Enter your email" required>
        </div>

        <div class="form-group">
            <label for="comments">Comments:</label>
            <textarea id="comments" name="comments" placeholder="Enter your comments, bad word is allowed" rows="5" required></textarea>
        </div>

        <button type="submit">Submit</button>
    </form>
</body>

</html>

```

--------

### Back-end Programming (PHP/ C#/ C++/ Dart) - Intermediate / Internal Training (HS)
**Session destroy is:** to terminate or clear a session, the example of implementation session destroy is at logout function.

```php
<?php
session_start();

if (isset($_SESSION['user'])) {
    unset($_SESSION['user']);

    // Destroy the session
    session_destroy();

    echo 'Session destroyed. User logged out.';
} else {
    echo 'No active session found.';
}
?>

```
