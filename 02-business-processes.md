# 2. Business Processes

## 2.1 Sale of an item
1. Cashier scans the product ID.
2. System checks that quantity > 0.
3. Bill is generated and stock quantity is reduced.

## 2.2 Automatic reorder
1. After every sale, system compares quantity with reorder level.
2. If `quantity <= reorder_level`, a draft purchase order is created.
3. Manager approves it and it is sent to the supplier.

## 2.3 Receiving stock
1. Supplier delivers goods against the purchase order.
2. Staff verify quantity and update stock.
3. Purchase order is marked **Closed**.

## Business Rules
- Stock can never be negative.
- Order quantity = `max_stock - current_quantity`.
- Every purchase order must be approved by the manager.
