Remaining tasks in Drupal:

- Complete the Score token by looping through submitted values.

Remaining tasks in React:

- List submissions
  - Create a SubmissionsOverview component based on the Overview component.
    - Main graphQL query will be a webformSubmissionQuery.
  - Create new SubmissionRow component, based on the ArticleTeaser component.
    - Query fragment will contain url, title, host entity name, score.
    - URL will be absolute URL to Drupal node.
  - SubmissionOverview and SubmissionRow will be formatted as a table instead of as teasers.
  - Update the Router component and query to include SubmissionOverview.
- Add filtering
  - On SubmissionsOverview, assemble list of webforms in a select list.
  - Selecting one webform sets a "selectedWebform" prop on the form, to pass to query.
  - Will require adding a filter to the query, and making sure that state management and property passing is set up properly.
- Display each submission in react
  - Create new Submission component, based on Article.
  - Expand graphQL fragment to get all fields needed for the detail display.
  - Keep url relative, and use the same system as Article for displaying the full submission.
