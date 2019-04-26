# Church calendar

## Description
- [ ] Simple web application, where you can add days to the list, modify its details.

## Entity definition
- [ ] Day:
   - [ ] id: number;
   - [ ] date: string; const lenth 10.
   - [ ] season: string; lenth 30.
   - [ ] season_week: string; const lenth 2.
   - [ ] weekday: string; max lenth 8
   - [ ] celebration: string; 
   - [ ] celebrations: string[];

## API definition
- [ ] POST /api/days
    - [ ] Creates new day.
    - 502 (Bad Gateway) if given day was invalid.
    - 202 if day posted.
    - 500 if some internal errors occured.
- [ ] GET /api/days
    - [ ] Gets all days.
    - Returns 200 (OK) list of all days.
    - Returns 200 with empty list if no days found.
    - Returns 404 (NotFound) if picture doesn't exist.
- [ ] GET /api/days/{id}
    - [ ] Gets day by id.
    - Returns 200 (OK) specific object by id.
    - Returns 404 (NotFound) if picture doesn't exist.
- [ ] UPDATE /api/days/{id}
    - [ ] Updates day by id.
     - 200 updated
     - 404 not found
- [ ] DELETE /api/days/{id}
    - [ ] Deletes day by id.
     - 200 deleted
     - 404 not found

## UI definition
Main view will be a list of added days. It will have an option to add specified day and to delete list items. Second view will be detailed view of the list selection, it will have an option to add a celebration and two buttons: to go back to listview and to save changes.
