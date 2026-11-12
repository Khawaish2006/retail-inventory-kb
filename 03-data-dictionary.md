# 3. Data Dictionary

| Entity | Field | Type | Description |
|--------|-------|------|-------------|
| Product | product_id | String | Unique product code |
| Product | name | String | Product name |
| Product | category | String | Product category |
| Product | price | Decimal | Selling price (INR) |
| Stock | quantity | Integer | Units currently in store |
| Stock | reorder_level | Integer | Minimum units before reordering |
| Stock | max_stock | Integer | Maximum units to hold |
| PurchaseOrder | po_id | String | Purchase order number |
| PurchaseOrder | supplier | String | Supplier name |
| PurchaseOrder | status | Enum | Draft / Approved / Closed |
