# Chemical Supplies Management PWA

## Overview

This project is a Progressive Web App (PWA) designed for managing chemical supplies. It allows users to add, edit, delete, and sort chemical entries in a dynamic table format. The application is built using HTML, CSS, and JavaScript and is optimized for both desktop and mobile use.

## Features

- **Dynamic Table**: Users can view, add, edit, delete, and sort chemical supplies in a table format.
- **Local Storage**: Data is stored in the browser's local storage, enabling persistence across sessions.
- **Service Worker**: A service worker is implemented to cache resources for offline use.
- **Responsive Design**: The UI is designed to be usable on both desktop and mobile devices.

## Design Approach

### 1. Structure

The application is structured in a modular fashion with separate files for HTML, CSS, JavaScript, and the service worker:

- **index.html**: Contains the structure and layout of the application.
- **styles.css**: Contains styles to enhance the appearance of the app.
- **script.js**: Contains the main logic for handling data manipulation and interactions.
- **service-worker.js**: Manages caching and offline capabilities.
- **manifest.json**: Provides metadata for the PWA.

### 2. User Interface

- **Table Layout**: The main feature is a table where chemical supplies are displayed. Each row contains relevant information such as ID, chemical name, vendor, density, viscosity, packaging, pack size, unit, and quantity.
- **Toolbar**: A toolbar above the table provides buttons for common actions: Add, Move Up, Move Down, Delete, Save, and Refresh.

### 3. Data Management

- **Local Storage**: The application uses the `localStorage` API to store chemical data. This allows users to retrieve their data even after closing the browser.
- **Default Data**: If no data is found in local storage, default sample data is loaded.
- **Data Editing**: Cells are editable. When a user clicks on a cell, it transforms into an input field, allowing inline editing.

### 4. Sorting Mechanism

- The table can be sorted by clicking on the column headers. The sorting function toggles between ascending and descending order, enhancing user experience.

### 5. User Interactions

- **Add Row**: Users can add a new empty row to the table.
- **Move Row**: Users can move a selected row up or down in the table.
- **Delete Row**: Users can delete selected rows.
- **Save Data**: Users can save their changes to local storage.
- **Refresh Data**: The refresh button reloads data from local storage, with a confirmation prompt if there are unsaved changes.

### 6. Offline Functionality

- The service worker caches essential files to allow the app to function offline. Users can still view their chemical supplies without an internet connection.

### 7. Responsiveness

- The layout and controls are designed to be responsive, ensuring a good user experience across different device sizes.

## Usage

1. Clone the repository or download the code.
2. Open `index.html` in a web browser. It is recommended to serve it using a local server for proper functionality.
3. Use the toolbar buttons to manage chemical supplies.

## Future Improvements

- Implement user authentication for multiple users.
- Allow importing/exporting of chemical data (e.g., CSV files).
- Add filtering options to narrow down search results in the table.

## License

This project is open source.
