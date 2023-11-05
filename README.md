# Wikipedia-like Online Encyclopedia

This project is a web-based encyclopedia, inspired by Wikipedia, that allows users to create, edit, and search for encyclopedia entries. It's built using Django and Markdown to provide a user-friendly and lightweight platform for storing and displaying encyclopedia entries.

# Background

**Wikipedia** uses a markup language called Wikitext for its encyclopedia entries. In this project, we use Markdown to make the creation and editing of encyclopedia entries more accessible. Entries are stored as Markdown files in the entries/ directory and are dynamically converted to HTML for display.

# Specification

  - **Entry Page**: Visiting `/wiki/TITLE` displays the contents of the encyclopedia entry with the title `TITLE`. If the entry doesn't exist, it shows an error page.
  - **Index Page**: Updates the index page to allow users to click on entry names and go directly to that entry.
  - **Search**: Allows users to search for entries using the search box in the sidebar. It redirects to the entry's page if there's an exact match or displays a list of results for partial matches.
  - **New Page**: Provides a way for users to create new encyclopedia entries with a title and Markdown content. Handles duplicate titles and saves new entries.
  - **Edit Page**: Users can edit the Markdown content of an entry. The existing content is pre-populated in a textarea.
  - **Random Page**: Clicking "Random Page" takes the user to a random encyclopedia entry.
  - **Markdown to HTML Conversion**: Converts Markdown content to HTML for display. You can use the python-markdown2 package for this.
