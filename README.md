# My Movie Collection Gallery

This project is a simple, self-contained web page designed to showcase a personal movie collection. It provides a visually appealing interface to browse through movies, search for specific titles, filter them by decade, and watch trailers or clips directly within the browser.

Key Features:
*   **Movie Listing:** Displays movies with their posters, titles, and release years in a grid layout.
*   **Search Functionality:** Allows users to search for movies by title or year.
*   **Decade Filtering:** Provides buttons to filter the movie collection by specific decades (e.g., 2020s, 2010s, 2000s, 1990s).
*   **Integrated Video Player:** Clicking on a movie card opens a modal window with an embedded video player to watch the movie's video file. It also supports subtitles.
*   **Responsive Design:** The gallery layout adjusts for different screen sizes.
*   **Animations:** Subtle animations are used to enhance the user experience.

## Project Structure

The entire application is contained within a single HTML file:

*   `movie_gallery.html`: This file includes the HTML structure for the page, CSS styles for presentation, and JavaScript code for all functionalities.
    *   **HTML:** Defines the layout of the movie gallery, search bar, filter buttons, and the modal video player.
    *   **CSS:** Contains all the styling rules, including theme colors, layout specifics, and responsiveness. It's embedded within `<style>` tags in the `<head>` section.
    *   **JavaScript:** Manages the movie data, displays movie cards, handles search and filtering logic, and controls the video player functionality. Movie data (including titles, years, paths to posters, video files, and subtitle files) is stored in a JavaScript array directly within this file.

## How to Use

1.  **Open the Gallery:**
    *   Simply open the `movie_gallery.html` file in a modern web browser (e.g., Chrome, Firefox, Safari, Edge).
2.  **Browse Movies:**
    *   Scroll through the displayed movie cards.
3.  **Search for Movies:**
    *   Use the search bar at the top to type in a movie title or year. The gallery will update in real-time to show matching results.
4.  **Filter by Decade:**
    *   Click on the decade buttons (e.g., "2020s", "2010s") to filter the movies displayed. Click "All" to see the entire collection.
5.  **Watch a Movie:**
    *   Click on any movie card. A modal window will appear with a video player.
    *   The video player has standard controls (play/pause, volume, fullscreen).
    *   If subtitles are available for a movie, they can be selected within the player.
    *   Click the "X" button on the modal or press the "Escape" key to close the video player.

## Dependencies / External Libraries

This project utilizes a few external libraries, all loaded via Content Delivery Networks (CDNs), so no local installation is required:

*   **Font Awesome:** Used for icons (e.g., search icon, play icon, close icon).
    *   Loaded from: `https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css`
*   **Anime.js:** A lightweight JavaScript animation library used for visual effects and transitions.
    *   Loaded from: `https://cdn.jsdelivr.net/npm/animejs@3.2.1/lib/anime.min.js`
*   **Video.js:** A comprehensive web video player.
    *   JS loaded from: `https://cdn.jsdelivr.net/npm/video.js@8.5.2/dist/video.min.js`
    *   CSS loaded from: `https://cdn.jsdelivr.net/npm/video.js@8.5.2/dist/video-js.min.css`

## Potential Future Enhancements

*   **External Movie Data:** Move the `movies` array from the inline JavaScript to a separate JSON file (e.g., `movies.json`). This would make it easier to manage and update the movie collection without directly editing the HTML file. The JavaScript would then fetch this JSON file to load the movie data.
*   **Separate CSS File:** Extract the CSS styles from the `<style>` tags into a dedicated `.css` file (e.g., `style.css`). This improves code organization and maintainability.
*   **Local Asset Hosting:** For offline use or more robust hosting, the movie posters, video files, and subtitle files could be hosted locally within the project structure instead of relying on potentially varied paths.
*   **Advanced Filtering/Sorting:** Implement more advanced filtering options (e.g., by genre, rating) or sorting capabilities (e.g., by title, year).
*   **User Authentication:** For a more personalized collection, user accounts and authentication could be added.
*   **Database Integration:** For larger collections, integrating a database (like SQLite or a more robust solution) could offer better data management and scalability.
