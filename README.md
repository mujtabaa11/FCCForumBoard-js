# freeCodeCamp Forum Leaderboard

## Overview

This project fetches and displays the latest topics from the freeCodeCamp forum, showing important details such as the topic title, the number of replies, views, last activity time, and user avatars. It uses a JSON endpoint to retrieve the data and dynamically generates a table of topics.

## Features

- **Topic List**: Displays the latest forum topics.
- **Category Links**: Each topic is associated with a category. Clicking the category takes you to the specific category page.
- **User Avatars**: Displays avatars of users who posted the topic.
- **Topic Stats**: Shows the number of replies, views, and the time of the last activity (e.g., minutes, hours, or days ago).
- **Responsive Design**: The application is designed to be responsive and adjusts well to smaller screen sizes.

## Technologies Used

- **Frontend**: HTML, CSS, JavaScript
- **API**: Fetches data from the [freeCodeCamp forum](https://forum.freecodecamp.org/)
- **Data Formatting**: Displays formatted data like time ago (in minutes, hours, or days) and view counts (abbreviated to 'k' for thousands).

## Project Structure

1. **HTML (`index.html`)**: The basic structure of the page, including the table that will display the forum posts.
2. **CSS (`styles.css`)**: Provides the styling and layout of the table and other components, including responsive design and colors for different categories.
3. **JavaScript (`script.js`)**: Handles the logic for fetching data from the freeCodeCamp API, formatting it, and displaying it in the table.

## Installation

### Prerequisites

- Make sure you have a browser to view the project.

### Steps

1. **Clone the Repository** (or download the files):
    ```bash
    git clone <repository_url>
    ```

2. **Open the project in your browser**:
    - Open `index.html` in any browser.

---

## How It Works

### JavaScript Logic
1. **Fetching Data**: The app fetches the latest forum posts using the `fetch` function from the [freeCodeCamp forum API](https://cdn.freecodecamp.org/curriculum/forum-latest/latest.json).
2. **Time Ago Function**: Converts the `bumped_at` timestamp into a human-readable format (e.g., "2h ago" or "3d ago").
3. **View Count Formatting**: If a post has over 1,000 views, it abbreviates the number with a 'k' (e.g., 1,200 views becomes "1k").
4. **Category Links**: Generates links for each category that lead to the corresponding category page on the freeCodeCamp forum.
5. **Dynamic Rendering**: Dynamically populates the table with data for each post, including the title, category, avatars of the posters, replies, views, and last activity time.

---

## Features in Detail

- **Category**: Each topic is associated with a category (e.g., "Career Advice", "JavaScript", "Python"). The categories are color-coded for easy identification.
- **Time Ago**: The app shows when a topic was last active (e.g., "5m ago", "2h ago", or "1d ago") based on the `bumped_at` timestamp.
- **User Avatars**: Avatars of the users who participated in the topic are displayed in a row, and are linked to their profile on the forum.
- **Responsive Design**: The layout adjusts based on screen size to ensure readability on smaller devices.

---

## License

This project is open-source and available under the [MIT License](./LICENSE).

---

## Future Enhancements

- **Pagination**: Implement pagination to load more posts.
- **Sorting**: Allow users to sort topics based on views, replies, or last activity.
- **Search Functionality**: Add a search feature to filter topics based on title or category.

---

Feel free to reach out if you have any questions or suggestions!
