
- Data was scraped from the GitHub API by filtering users in Basel with over 10 followers and fetching their most recent repositories.

- A significant portion of repositories in Basel are written in JavaScript but surprisingly PHP is also seen in many repositories.

- Developers in Basel should focus on collaboration in JavaScript-based and Python-based projects to leverage the local expertise and community.





## How the Data Was Collected

1. **API Endpoints**:
   - `GET /search/users`: Used to locate users in Basel with more than 10 followers.
   - `GET /users/{username}`: Collected detailed information for each user.
   - `GET /users/{username}/repos`: Listed up to 500 repositories per user.

2. **Data Processing**:
   - **Company Cleanup**: Trimmed whitespace, removed symbols, and standardized names to uppercase.
   - **Empty Fields**: Replaced null values with empty strings.