# Household Health
This is an example application that provides a way to capture information about a household applying for health insurance coverage. 

## Try it out!
https://nym.github.io/household-health/

## Acceptance Criteria:
[X] Validate data entry (age is required and > 0, relationship is required)
[X] Add people to a growing household list
[X] Remove a previously added person from the list
[X] Display the household list in the HTML as it is modified
[X] Serialize the household as JSON upon form submission as a fake trip to the server

## Requirements: 
- Do not modify HTML
- Do not make UI pretty
- No external libaries

## Implementation Notes:
The way I approached this exercise was to treat this as challenge of managing state instead of focusing on presentation. Following my experience using React and Redux, I built a basic flux pattern, and components that would update only when the state was changed (one-way data flow / binding). Additionally, components can ignore state changes if the data wouldn't affect the rendered result.