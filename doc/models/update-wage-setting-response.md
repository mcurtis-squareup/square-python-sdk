
# Update Wage Setting Response

Represents a response from an update request containing the updated `WageSetting` object
or error messages.

## Structure

`Update Wage Setting Response`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `wage_setting` | [`Wage Setting`](../../doc/models/wage-setting.md) | Optional | An object representing a team member's wage information. |
| `errors` | [`List of Error`](../../doc/models/error.md) | Optional | The errors that occurred during the request. |

## Example (as JSON)

```json
{
  "wage_setting": {
    "created_at": "2019-07-10T17:26:48+00:00",
    "is_overtime_exempt": true,
    "job_assignments": [
      {
        "annual_rate": {
          "amount": 3000000,
          "currency": "USD"
        },
        "hourly_rate": {
          "amount": 1443,
          "currency": "USD"
        },
        "job_title": "Manager",
        "pay_type": "SALARY",
        "weekly_hours": 40
      },
      {
        "hourly_rate": {
          "amount": 1200,
          "currency": "USD"
        },
        "job_title": "Cashier",
        "pay_type": "HOURLY"
      }
    ],
    "team_member_id": "-3oZQKPKVk6gUXU_V5Qa",
    "updated_at": "2020-06-11T23:12:04+00:00",
    "version": 1
  }
}
```

