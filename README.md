# api-standards

This is Freighthub API guidelines, forked from PayPal

You can find the actual **guidelines** [here](https://github.com/freight-hub/api-standards/blob/master/api-style-guide.md)

You can find **examples** and **patterns** [here](https://github.com/freight-hub/api-standards/blob/master/patterns.md)

You can find the list of **references** [here](https://github.com/freight-hub/api-standards/blob/master/references.md)

You can find the **JSON schema** spec [here](https://github.com/freight-hub/api-standards/tree/master/v1/schema/json/draft-04)

## TL;DR

**Paths**: kebab case and plurals ✅ `purchase-orders` 🚫`purchaseOrder`, `purchaseOrders`, `purchase_orders`

**Query Params**: camelCase ✅ `customerID` 🚫`customer-id`, `customer_id`, `customerId`

**Path Params**: camelCase ✅ `customerID` 🚫`customer-id`, `customerId`

**Headers**: Pascal-Case, no X- for custom headers ✅ `API-Key` 🚫`api-key`, `apiKey`, `X-API-Key`

**Responses**: must be an object with camelCase properties ✅ `customerID`, `id` 🚫`customer-id`,`customerID`, `_id`

**Pagination**: must take `page` and `pageSize` parameters and response must contains a property `items` and should contain `totalItems` for the respones (also accepted is `totalPages`)

**Enums**: must be camcelCase ✅ `green`, `blue`, `blueGreen` 🚫 `BLUE`, `blue_green`

**Abbreviations/Acronyms**: must be all lower or all upper case  ✅ `HTTP`, `API`, `{ "id": 1 }` 🚫 `Http`, `Api`
