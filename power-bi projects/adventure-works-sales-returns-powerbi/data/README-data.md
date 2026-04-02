# Data — Adventure Works Sales & Returns Analysis

## Source

The Adventure Works dataset is a publicly available Microsoft sample dataset commonly used for
business intelligence and data analytics demonstrations.

## Dataset Structure

The project uses the following source CSV files:

| File | Description |
|---|---|
| `Sales_Data.csv` | Transactional sales records including CustomerKey, OrderDate, ProductKey, OrderQuantity, RetailPrice |
| `Returns_Data.csv` | Product return records including ReturnDate, ProductKey, ReturnQuantity, TerritoryKey |
| `Customer_Lookup.csv` | Customer demographics including AnnualIncome, BirthYear, CustomerPriority, Occupation |
| `Product_Lookup.csv` | Product details including ProductName, ModelName, ProductCost, ProductPrice |
| `Product_Categories_Lookup.csv` | Product category hierarchy (Bikes, Accessories, Clothing) |
| `Product_Subcategories_Lookup.csv` | Product subcategory mapping |
| `Territory_Lookup.csv` | Geographic territories including Country, Region, Continent |

## Data Volume

- **Period covered:** January 2020 – June 2022
- **Total Orders:** ~25,000
- **Unique Customers:** ~17,000
- **Regions:** North America, Europe, Pacific

## Notes

The raw CSV files are not included in this repository as the Adventure Works dataset
is publicly available from Microsoft and can be downloaded directly from the official
Microsoft learning resources.

The data was loaded, cleaned, and transformed entirely within Power BI using Power Query (M language).
No external Python or SQL processing was required.
