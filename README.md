# Funny Jokes Website

A simple web application that fetches and displays funny dad jokes from [icanhazdadjoke.com](https://icanhazdadjoke.com/).

## Features

- Fetches random jokes using the Dad Jokes API
- Responsive design

## Technologies Used

- HTML
- CSS
- JavaScript

## Usage

Click the "Next Joke" button to fetch a random dad joke and enjoy the laughs!

## Example Code

Fetch a joke with:
```
fetch('https://icanhazdadjoke.com/', {
    headers: {
        'Accept': 'application/json'
    }
})
.then(response => response.json())
.then(data => {
    document.getElementById('joke').innerText = data.joke;
})
.catch(error => console.error('Error fetching joke:', error));
```

