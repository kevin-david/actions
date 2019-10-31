# Archive Project Board javascript action

Goes through the last column of a project board and archives any issues which have not been been updated since archive-period-days

## Inputs

### `organization`

**Required** The organization which the project belongs to.

### `project`

**Required** The project board #.

### `token`

**Required** PAT token with access to the board - must be a secret.

### `archive-period-days`

**Required** The number of days since the issue has been last updated to consider it for archival. Default 14 days.

## Outputs

### `archived-items`

The # of items which were archived.

## Example usage

uses: actions/hello-world-javascript-action@v1
with:
  who-to-greet: 'Mona the Octocat'