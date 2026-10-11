# Initial Data Dictionary

This describes the current browser prototype and a future synthetic analytics model. It is not authorization to collect real health data.

## Browser check-in record

| Field | Type | Required | Meaning | Notes |
|---|---|---:|---|---|
| `date` | ISO-like date string | Yes | Local calendar date for the entry | One entry per date; browser locale behavior should be tested |
| `mood` | Categorical string | No | User-selected mood label | Not a clinical assessment |
| `intention` | Categorical string | No | User-selected daily intention | Not a treatment plan |
| `trigger` | Categorical string | No | Optional user-selected influence | Sensitive context; keep optional |
| `note` | String, max 400 characters | No | Private reflection | Avoid names and identifying details |

## Storage and privacy

- Current implementation uses browser `localStorage` on the device.
- No network request or backend persistence is implemented in this prototype.
- Anyone with access to the same browser profile may be able to view local entries.
- Export produces a JSON file on the user's device; that file may be sensitive.
- Delete removes the app's local key in that browser. It does not delete exported copies.
- Do not add real personal or health information to GitHub, screenshots, issues, or public demo datasets.

## Synthetic analytics model (future)

A separate, synthetic dataset may include generated participant IDs, dates, feature events, and usability ratings. Clearly label generated data as synthetic. Do not combine synthetic rows with real participants in a way that misrepresents the source. Any future research dataset needs a separate data protection and consent plan.

## Data quality checks to implement

1. Date values parse and fall within the test window.
2. Mood and intention values match documented categories.
3. Optional fields may be empty.
4. Notes stay within the character limit.
5. Duplicate dates are handled according to the one-entry-per-day rule.
6. Missingness and exclusions are reported in analysis.
7. Dashboards show metric definitions and denominators.
