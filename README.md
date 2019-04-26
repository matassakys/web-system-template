# Church calendar

## Description
- [ ] Simple web application, where you can add days to the list, modify its details.

## Entity definition
- [ ] Day:
    id: number;
    date: string;
    season: string;
    season_week: string;
    weekday: string;
    celebration: string;
    celebrations: string[];

## API definition
- [ ] POST /api/days
    - [ ] Creates new day.
- [ ] GET /api/days
    - [ ] Gets all days.
- [ ] GET /api/days/{id}
    - [ ] Gets day by id.
- [ ] UPDATE /api/days/{id}
    - [ ] Updates day by id.
- [ ] DELETE /api/days/{id}
    - [ ] Deletes day by id.

## UI definition
Main view will be a list of added days. It will have an option to add specified day and to delete list items. Second view will be detailed view of the list selection, it will have an option to add a celebration and two buttons: to go back to listview and to save changes.
