Here's the English translation of the provided text, maintaining the original structure and emphasis:

Search Features
Keyword Search: Users can enter a query to search for relevant websites.

Stop Word Filtering: It can be configured to ignore common words (stop words) during the search to improve relevance, by loading them from a specified source.

Synonym Expansion: The search can automatically expand queries with synonyms to broaden search results.

Result Limitation: Users can configure the maximum number of search results to display.

Typo Correction/Suggestion: If no results are found, the application attempts to suggest the "closest" matching word from its index using the Levenshtein distance algorithm, helping users with potential typos.

Performance Metrics: Displays the number of results found and the time taken for the search.

Web Navigation
Integrated Web Browser: Offers a functional web browser directly within the Swing application.

Navigation Buttons: Includes "Back" and "Forward" buttons for navigating web Browse history.

Website Information Display: Shows the "Site Name" instead of just the raw URL in the search results list, which is more user-friendly.

Dynamic UI Switching: Smoothly switches between the search results view and the web content view.

User Interface (Swing)
Responsive Design: Font sizes dynamically adjust based on window resizing for a better user experience across different screen sizes.

Event Handling: Implements ActionListener for button clicks and MouseAdapter for list item selection.

Custom Settings Dialog: A separate ParametresGUI JDialog allows users to configure search settings.

Configuration and Data Management
Configurable Settings: Allows users to enable/disable stop words and synonyms, set the maximum number of results, and control data collection via a dedicated "Settings" window.

Persistent Settings: Saves and loads user settings (stop word usage, synonym usage, maximum results, data collection) from a "config.properties" file, ensuring preferences are retained across sessions.

Architectural Aspects
MVC-like UI Structure: Although not a strict MVC implementation, there is a separation of concerns, with RechercheGUI handling the main view and control, and SiteInfo acting as a simple model for search results.

Error Handling: Includes basic try-catch blocks for file I/O operations and numeric parsing to gracefully handle potential errors.
