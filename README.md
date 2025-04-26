# BrickBuddy API Docs Demo

> **Demo project for the Pluralsight course _"Creating Developer Documentation with GitHub Copilot"_**

---

## Overview

This project demonstrates how to document and test a simple API using modern developer tools. It features a Node.js/Express backend and a React-based frontend for interactive API exploration. All data and endpoints are mock/demo only.

---

## Quick Start

```bash
# Install dependencies
npm install

# Start the backend server
npm start
```

The server will run on [http://localhost:5001](http://localhost:5001) by default.

---

## API Usage Example

**Endpoint:**
```
GET /api/piece-destinations?lot_id=YOUR_LOT_ID
```

**Query Parameters:**
- `lot_id` (required): The ID of the lot to fetch destinations for.

**Sample Response:**
```json
{
  "set_destinations": [
    { "name": "Demo Set 1", "number": "75300-1", ... },
    { "name": "Demo Set 2", "number": "10281-1", ... }
  ],
  "part_destinations": [
    { "recommended": true, "user_inventory_item_location_name": "Parts Drawer 5", ... },
    { "recommended": false, "user_inventory_item_location_name": "Bulk Parts Tub", ... }
  ]
}
```

## Notes

- This project is for demonstration and educational purposes only. All data is mock data.
- For OpenAPI integration, place your OpenAPI YAML files in an `openapi/` directory at the project root.

---

## License

MIT 