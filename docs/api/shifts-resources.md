---
layout: page
---
# `shifts` resource

Base endpoint:

```shell
{server_url}/shifts
```

Contains information about the shifts saved to the Who's Working service. In Version 1, only registered store managers can create a shift.

## Resource properties

Sample `shifts` resource.

```js
{
    "id": "81a2",
    "date": "2024-06-11",
    "start_time": "0900",
    "shift_length": "6",
    "warning": "opening",
    "location_detail": "Eatons Centre",
    "status": "closed"
}
```

| Property name | Type | Description |
| ------------- | ----------- | ----------- |
| `id`     | number | The unique ID assigned to the shift.  |
| `date`    | string | The date (YYYY-MM-DD) of the work shift. Use the [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format.|
| `start_time` | integer | The shift's start time. Use 24 clock time with no colon.|
| `shift_length` | decimal | The shift length is measured in hours. Use numbers with one decimal place (e.g. 4.5).|
| `warning`     | number | The number of hours and minutes relative to the `date` to alert workers of the shift. This is normally a negative number to alert the user before the `date`. |
| `location_detail`  | string | A short description of the restaurant's location.|
| `status`  | string | The shift is **Open** (waiting to fill the position) or **Closed** (the position is no longer available).|

## Operations

The `shifts` resource supports these operations.

### READ (GET)

* [Get shifts by status](get-shifts-by-status)
* Get all shifts
* Get shift by ID
* Get shifts by date
* Get shifts by shift length
* Get shifts by location detail


### CREATE (POST)

* [Create a shift](create-shift)

### UPDATE (PUT/PATCH)

* [Change shift status](change-shift-status)
* Update shift by ID
* Change shift date

### DELETE

* [Delete a shift by ID](delete-shift-by-id)
