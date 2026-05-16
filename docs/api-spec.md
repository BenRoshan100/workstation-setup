# API Specification — [Project Name]

## Base URL
`https://[your-project].railway.app`

## Endpoints

### POST /score
**Purpose:** [describe]
**Request:**
```json
{
  "field": "type"
}
```
**Response:**
```json
{
  "result": "type"
}
```
**Example curl:**
```bash
curl -X POST https://[url]/score \
  -H "Content-Type: application/json" \
  -d '{"field": "value"}'
```

### GET /health
**Purpose:** Health check
**Response:** `{"status": "ok", "version": "1.0.0"}`
