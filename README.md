# 🌍 English | [简体中文](README.zh-CN.md)

# Cross-Border DTC Inventory Governance Console
### Demand Signal Cleansing, Pre-order Liability Control, and Purchase Planning for Shopify-Based Brands

![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)
![Platform](https://img.shields.io/badge/Platform-Browser%20%7C%20Excel-success)
![Tool](https://img.shields.io/badge/Tool-Inventory%20Decision%20Support-orange)

**Turn noisy Shopify order data into purchasing decisions in minutes—directly in a browser or Excel workbook, with no signup, no installation, and no recurring subscription.**

> ## ✅ No signup. No installation. Free.
>
> 🌐 **Open in Browser**  
> *(HTML Live Version – Coming Soon)*
>
> 📥 **Download Excel Version**  
> *(GitHub Release / Gumroad Download)*

---

# Screenshots

### Browser Version

<!-- screenshot: browser version -->

> Displays demand cleansing, purchase recommendations, pre-order liabilities, and inventory allocation in a browser without requiring Excel.

---

### Excel Version

<!-- screenshot: excel version -->

> Complete workbook including data import sheets, analytical engine, reconciliation, purchasing recommendations, and executive dashboard.

---

# What It Helps You Track

Instead of looking at disconnected reports from Shopify, Inventory Planner, and spreadsheets, this console brings the operational signals together into one decision framework.

It makes it possible to see:

- Outstanding pre-order liabilities that should not be counted as available inventory.
- True demand after removing pre-order distortion and expected returns.
- Purchase quantities that reflect actual inventory obligations instead of inflated sales.
- Inventory allocation across UK, US, EU, and AUS based on demand contribution.
- Synchronization gaps between Shopify, Inventory Planner, and purchasing records before they become planning mistakes.
- Weekly purchasing priorities supported by reconciled operational data instead of manual spreadsheet adjustments.

---

# Quick Start Workflow

The workbook is designed around a **configure once, refresh regularly** workflow rather than constant spreadsheet maintenance.

### 1. Configure Operational Parameters

Open the **Config** worksheet and define operational rules such as:

- Lead time
- Return window
- Market allocation ratio
- Pre-order safety factor

These values usually change only when business policies change.

---

### 2. Import Existing Business Data

Export existing operational data from Shopify and Inventory Planner.

Paste or refresh:

- Shopify Orders
- Shopify Returns
- Current Inventory
- Purchase Status

No restructuring or manual formula updates are required.

---

### 3. Review Automatically Updated Decisions

Navigate directly to the analytical sheets.

The workbook immediately refreshes:

- Outstanding Pre-order Liability
- Cohort Return Analysis
- Corrected Demand
- Purchase Recommendations
- Country Allocation
- Reconciliation Status

No manual calculations are needed.

---

### 4. Refresh Weekly

Each planning cycle simply replaces the raw input tables.

Everything downstream updates automatically.

There is no workbook rebuilding, formula copying, or structural maintenance.

**Set a few operational parameters. Import existing data. Review the recommendations. Refresh whenever new business data becomes available.**

---

# Why I Built This

Many inventory planning problems are not caused by poor forecasting algorithms.

They are caused by poor demand signals.

For brands operating multiple Shopify storefronts, especially fashion businesses with heavy pre-orders and high return rates, reported sales often contain signals that should never become purchasing demand.

A pre-order is recorded as a sale before inventory exists.

A returned item may not re-enter inventory until weeks later.

Inventory planners frequently receive historical sales without understanding either condition.

The result is predictable:

- purchasing twice for the same demand,
- overestimating future inventory requirements,
- accumulating unnecessary stock,
- increasing working capital without increasing revenue.

I built this project because I repeatedly observed analysts spending hours cleaning data before they could even begin making purchasing decisions.

Instead of creating another dashboard, I wanted to package the reasoning process itself into a reusable workbook.

For example:

**Before**

A SKU sells **500 units** during a launch.

Traditional planning assumes demand equals 500.

Purchase recommendations are generated from that number.

---

**After**

The workbook discovers:

- 120 units are still unfulfilled pre-orders.
- Expected returns equal 48 units.
- Corrected demand becomes **332 units**.

The purchasing conversation changes immediately.

Instead of discussing how quickly to reorder 500 units, operations teams discuss whether 332 units are sufficient after accounting for lead time and safety stock.

That is a fundamentally different decision—not because the formulas changed, but because the demand signal became trustworthy.

---

# Common Inventory Planning Problems This Solves

| Problem | Without This Tool | With This Tool |
|----------|-------------------|----------------|
| Pre-orders inflate demand | Purchases duplicate already committed inventory | Outstanding liabilities are isolated before forecasting |
| Returns distort historical sales | Forecasts assume all sales become permanent demand | Cohort return modelling estimates recoverable inventory |
| Multiple countries compete for inventory | Manual allocation creates inconsistent stock levels | Allocation follows configurable market contribution ratios |
| Purchasing decisions rely on disconnected systems | Analysts compare Shopify, Inventory Planner and ERP manually | Automated reconciliation highlights mismatched quantities |
| Weekly planning requires rebuilding spreadsheets | Formula copying introduces hidden errors | Raw data is refreshed while calculations remain unchanged |
| Inventory issues are discovered too late | Purchasing errors appear after PO creation | Reconciliation exposes discrepancies before orders are issued |

---

# Who This Is For

This project is designed for organizations managing inventory decisions across multiple markets where demand signals are influenced by pre-orders, returns, and international fulfilment.

Typical users include:

- DTC fashion brands
- Shopify operations teams
- Inventory planners
- Supply chain analysts
- Merchandise planning teams
- Ecommerce operations managers

It is particularly valuable where purchasing decisions depend on understanding the difference between **reported sales** and **real inventory demand**.

It is **not** intended to replace ERP platforms, warehouse management systems, or enterprise inventory software.

Instead, it provides a lightweight analytical layer between operational systems and purchasing decisions.

No spreadsheet expertise is required. Open the browser version or Excel workbook, import operational data, and begin reviewing purchasing recommendations immediately.

---

# About

I build lightweight analytical workbooks for business situations where there are simply too many moving parts to reason through mentally.

Rather than replacing enterprise software, these tools organize the information needed to make the next operational decision with confidence.

The **Cross-Border DTC Inventory Governance Console** is one example of this approach: transforming fragmented operational data into a repeatable decision-support framework that can be refreshed whenever new information becomes available.

## Technical Details

<details>
<summary><strong>For technical reviewers, Excel practitioners, and collaborators</strong></summary>

---

# Workbook Architecture

The workbook follows a strict **Input → Cleansing → Decision → Validation → Output** architecture. Each worksheet has a single responsibility, making the analytical process transparent and auditable.

| Layer | Worksheet | Purpose | Output Consumer |
|--------|-----------|---------|-----------------|
| Configuration | Config | Business rules, lead time, allocation ratios, return window | All calculation sheets |
| Raw Input | Raw_Orders | Shopify order exports | Demand engine |
| Raw Input | Raw_Returns | Shopify return exports | Return model |
| Cleansing | Preorder_Liability | Outstanding pre-order obligations | Corrected Demand, PO Planner |
| Cleansing | Cohort_Return_Model | Cohort-based return behaviour | Corrected Demand |
| Decision | Corrected_Demand | True purchasing demand | Inventory Planner |
| Decision | PO_Planner | Purchase recommendations | Purchasing team |
| Decision | Location_Allocator | Country allocation | Warehouse & Logistics |
| Validation | Reconciliation | Cross-system verification | Operations |
| Presentation | Executive_Dashboard | Executive KPIs | Management |

### Overall Data Flow

```text
Shopify Orders
                     \
                      \
                       --> Raw_Orders ------------------\
                                                        \
                                                         \
Inventory Planner Export --> Current Inventory -----------> PO Planner
                                                          /
                                                         /
Shopify Returns --> Raw_Returns --> Cohort Return Model-/

                     Config Parameters
                             │
                             ▼
                 Preorder Liability Engine
                             │
                             ▼
                 Corrected Demand Engine
                             │
                             ▼
                Purchase Recommendation
                             │
                             ▼
                  Country Allocation
                             │
                             ▼
                    Reconciliation
                             │
                             ▼
                 Executive Dashboard
```

Unlike traditional spreadsheets where calculations are scattered across multiple worksheets, this workbook separates operational responsibilities into independent analytical layers.

That separation allows every purchasing recommendation to be traced back to its originating operational data.

---

# Three Analytical Traps That Catch Even Experienced Inventory Planners

---

## Trap 1 — Treating Pre-orders as Completed Demand

### Decision

The purchasing team increases production after observing unusually strong sales.

### Hidden Assumption

Reported sales are assumed to represent fulfilled customer demand.

In reality, a large proportion of those sales are still outstanding pre-orders.

### Why This Changes the Recommendation

| Metric | Traditional View | Corrected View |
|---------|-----------------|----------------|
| Sales | 1,000 | 1,000 |
| Outstanding Pre-orders | ignored | 280 |
| Purchasing Demand | 1,000 | 720 |

Without separating outstanding liabilities, inventory planners purchase products that customers have already committed to buying.

This creates duplicate purchasing.

### Why The Reasoning Is Wrong

Sales describe commercial activity.

Purchasing should respond to physical inventory obligations.

Those are not always the same thing.

Especially for fashion launches, crowdfunding, and long manufacturing lead times.

### Corrected Approach

Outstanding pre-orders are isolated before demand enters the purchasing model.

Only fulfilled demand contributes to future purchasing requirements.

### Decision Outcome

Instead of increasing production by 1,000 units,

operations purchase inventory for approximately 720 units,

reducing unnecessary inventory investment while still protecting customer commitments.

<details>
<summary>Formula Logic</summary>

```excel
Outstanding Liability

=
Total Preorder Sold
-
Fulfilled Preorders
```

Implemented using dynamic array formulas and SUMIFS.

</details>

---

## Trap 2 — Measuring Returns by Calendar Month

### Decision

Management concludes that return rates have fallen because this month's returns appear lower.

### Hidden Assumption

Returns occurring during a calendar month belong to sales made during that same month.

That assumption is almost never true.

Returns are tied to purchase cohorts rather than reporting periods.

### Why This Changes the Recommendation

Example:

| Month | Sales | Calendar Returns |
|--------|-------|-----------------|
| January | 8,000 | 220 |
| February | 6,500 | 640 |

Traditional reporting suggests February products perform worse.

However, most February returns actually belong to January purchases.

### Why The Reasoning Is Wrong

Customer behaviour follows order age.

Reports follow calendar dates.

Those timelines rarely align.

### Corrected Approach

Orders are grouped by purchase cohort.

Returns are measured:

- within 14 days
- within 30 days
- within 45 days

The resulting return profile reflects actual customer behaviour instead of reporting artefacts.

### Decision Outcome

Instead of reducing February purchasing,

the company discovers that January products experienced delayed returns,

while February demand remains healthy.

<details>
<summary>Formula Logic</summary>

```excel
Unique Cohort Months

=SORT(
UNIQUE(
TEXT(Order_Date,"yyyy-mm")
))
```

Combined with MAP(), LET(), and SUMIFS() to calculate return windows dynamically.

</details>

---

## Trap 3 — Purchasing From Raw Sales Instead of Corrected Demand

### Decision

Inventory Planner receives exported historical sales.

Forecasts appear reasonable.

Purchasing still creates excess inventory.

### Hidden Assumption

Historical sales already represent clean demand.

They rarely do.

Historical sales often include:

- outstanding pre-orders
- expected returns
- temporary launch spikes

### Before

```text
Historical Sales

980
```

Inventory Planner forecasts from 980.

### After Cleansing

```text
Historical Sales          980

Outstanding Liability    -170

Expected Returns          -62

Corrected Demand          748
```

### Why The Reasoning Is Wrong

Forecasting algorithms amplify input quality.

They cannot repair poor historical signals.

Garbage in still produces confident-looking garbage out.

### Corrected Approach

Demand is corrected before entering forecasting software.

Inventory Planner receives purchasing demand rather than commercial activity.

### Decision Outcome

Purchase recommendations become significantly more stable.

Working capital decreases while maintaining customer service levels.

<details>
<summary>Formula Logic</summary>

```excel
Corrected Demand

=
Raw Sales
-
Outstanding Liability
-
Expected Returns
```

Implemented using LET(), XLOOKUP(), SUMIFS(), and dynamic arrays.

</details>

---

# Example Scenario

A UK-based fashion brand launches a new jacket across four Shopify storefronts serving the UK, US, EU, and Australia.

Within two weeks, Shopify reports **2,450 units sold**, suggesting a highly successful launch. Based on raw sales alone, the purchasing team considers placing an urgent replenishment order.

The workbook tells a different story.

First, the **Preorder_Liability** sheet identifies **540 units** that have been sold but not yet fulfilled. These represent existing customer commitments rather than additional market demand.

Next, the **Cohort_Return_Model** evaluates historical return behaviour for comparable products. Previous launches show an ultimate return rate of **11.8%**, indicating that approximately **289 units** are expected to return to inventory after delivery.

The **Corrected_Demand** engine then recalculates the purchasing signal:

| Item | Quantity |
|------|---------:|
| Reported Sales | 2,450 |
| Outstanding Pre-orders | -540 |
| Expected Returns | -289 |
| Corrected Demand | **1,621** |

Rather than purchasing against the headline sales figure, the **PO_Planner** uses the corrected demand together with lead time, current stock, and safety parameters to recommend a significantly smaller replenishment quantity.

The recommendation is automatically distributed across the UK, US, EU, and AUS warehouses according to configured allocation ratios.

Finally, the **Reconciliation** worksheet compares Shopify liabilities with Inventory Planner synchronization data. If outstanding obligations differ between systems, the workbook raises an **INVESTIGATE** warning before purchase orders are issued.

The result is a purchasing decision supported by reconciled operational evidence instead of raw sales totals, reducing excess inventory while maintaining customer fulfilment commitments.
---

### Formula Reference

<details>
<summary>Config Sheet</summary>

| Formula / Logic | Purpose | Notes |
|-----------------|---------|------|
| Manual configuration | Defines operational parameters | Maintained only when business rules change |
| Market Allocation Ratio | Country inventory allocation | Used by Location_Allocator |
| Lead Time | Purchase planning | Included in target inventory calculation |
| Return Window | Cohort analysis | Controls expected return timing |
| Pre-order Safety Factor | Purchase buffer | Adjustable by market |

</details>

---

<details>
<summary>Preorder_Liability</summary>

### Generate Unique SKU List

```excel
=SORT(
UNIQUE(
Raw_Orders[SKU]
))
```

**Purpose**

Creates a dynamic SKU master list directly from imported order history.

---

### Outstanding Pre-order Liability

```excel
=LET(

SKU_List,A2#,

Preorder_Sold,

SUMIFS(
Raw_Orders[Quantity],
Raw_Orders[SKU],SKU_List,
Raw_Orders[Sales_Type],"Preorder"
),

Preorder_Fulfilled,

SUMIFS(
Raw_Orders[Quantity],
Raw_Orders[SKU],SKU_List,
Raw_Orders[Sales_Type],"Preorder",
Raw_Orders[Fulfillment_Status],"Fulfilled"
),

Preorder_Sold-
Preorder_Fulfilled

)
```

**Purpose**

Calculates inventory obligations that have already been sold but not physically delivered.

These quantities are intentionally excluded from future purchasing demand.

---

</details>

---

<details>
<summary>Cohort_Return_Model</summary>

### Generate Cohort Months

```excel
=SORT(
UNIQUE(
TEXT(
Raw_Orders[Order_Date],
"yyyy-mm"
)
))
```

---

### Cohort Return Calculation

Implemented with

- LET()
- MAP()
- SUMIFS()

The calculation measures returns relative to the original order date rather than calendar reporting periods.

Return windows include:

- 14 Days
- 30 Days
- 45 Days

This produces a stable estimate of ultimate return behaviour.

---

### Ultimate Return Rate

```text
Ultimate Return Rate

=

Total Returned Quantity

/

Original Cohort Sales
```

The workbook uses cohort-level behaviour instead of monthly return percentages because purchasing decisions depend on customer behaviour rather than reporting periods.

</details>

---

<details>
<summary>Corrected_Demand</summary>

### Corrected Demand Signal

```excel
=LET(

RawSales,

SUMIFS(...),

Outstanding,

XLOOKUP(...),

ExpectedReturns,

RawSales*
AverageReturnRate,

ROUND(

RawSales
-
Outstanding
-
ExpectedReturns,

0)

)
```

### Purpose

Transforms commercial activity into purchasing demand.

Instead of forecasting directly from historical sales, the workbook removes:

- Outstanding pre-orders
- Expected inventory returning through customer returns

The resulting signal is suitable for Inventory Planner or similar forecasting software.

</details>

---

<details>
<summary>PO_Planner</summary>

### Net Purchase Requirement

```text
Net Requirement

=

Target Inventory

-

Current Stock

+

Outstanding Liability
```

---

### Recommended Purchase Quantity

```excel
=IF(

NetRequired<=0,

0,

MROUND(

NetRequired,

MOQ

)

)
```

### Purpose

Automatically recommends purchase quantities while respecting supplier minimum order quantities.

Rather than requiring manual rounding, purchase recommendations are immediately suitable for issuing purchase orders.

</details>

---

<details>
<summary>Location_Allocator</summary>

### Country Allocation

```excel
=ROUND(

Total_PO

*

Allocation_Ratio,

0
)
```

Each destination warehouse receives inventory according to configurable market contribution ratios.

The allocation model can easily be expanded to additional countries without changing downstream calculations.

</details>

---

<details>
<summary>Reconciliation</summary>

### Synchronization Check

```excel
=IF(

Gap=0,

"PASS",

"INVESTIGATE"

)
```

where

```text
Gap

=

Shopify Unfulfilled

-

Inventory Planner Liability
```

Purpose:

Immediately highlights synchronization problems before purchasing decisions rely on inconsistent data.

</details>

---

## Validation Rules

| Field | Validation Rule | Error Behaviour |
|------|-----------------|----------------|
| Market | Must exist in Config table | Lookup returns default allocation or validation warning |
| SKU | Cannot be blank | Row excluded from calculations |
| Order_ID | Must be unique | Duplicate transaction warning |
| Return_ID | Must be unique | Duplicate return warning |
| Order Date | Valid date required | Record ignored until corrected |
| Return Date | Cannot precede Order Date | Validation flag generated |
| Quantity | Must be greater than zero | Row excluded |
| Return Quantity | Cannot exceed original quantity | Validation warning |
| Sales Type | Normal or Preorder only | Invalid category highlighted |
| Fulfillment Status | Fulfilled / Unfulfilled | Invalid values excluded |
| Allocation Ratio | Total must equal 100% | Country allocation warning |
| Lead Time | Non-negative integer | Purchase calculation halted |
| Return Window | Positive integer | Cohort calculation warning |
| MOQ | Greater than zero | Purchase recommendation disabled |
| Current Inventory | Cannot be negative | Inventory warning |
| Outstanding Liability | Cannot exceed preorder sales | Reconciliation alert |
| Recommended Purchase Quantity | Rounded to MOQ | Automatically adjusted |
| Synchronization Gap | Must equal zero | INVESTIGATE status displayed |

---

## Other Tools in This Series

These workbooks follow the same design philosophy: lightweight decision-support systems built for recurring operational problems rather than enterprise software replacement.

- **Inventory Forecasting & Reorder Planning** — Demand forecasting, reorder point calculation, and inventory risk analysis.
- **Construction Estimating System** — Estimating assemblies, cost libraries, bid preparation, and project budgeting.
- **Marketing Budget Allocation Simulator** — Scenario planning for multi-channel marketing investment.
- **Multi-Currency Trade Finance Dashboard** — Cross-border financial reporting and profitability analysis.
- **Coffee Shop Operations Audit Toolkit** — Store performance review and operational compliance analysis.
- **Project Management & Progress Billing Console** — Milestone tracking, invoicing, and budget control.

More analytical workbooks will be published through the GitHub repository and Gumroad download library.

---

## License

This project is licensed under the **Apache License 2.0**.

You are free to:

- Use the workbook for personal or commercial purposes.
- Modify the analytical framework to suit operational requirements.
- Distribute modified versions in accordance with the Apache License 2.0.

See the **LICENSE** file for the complete license text.

---

## Final Notes

This workbook is intentionally positioned as a **decision-support layer**, not as a replacement for ERP, WMS, or enterprise planning platforms.

Its purpose is straightforward:

- capture operational data from existing systems,
- remove analytical distortions before planning,
- generate purchasing recommendations that reflect real inventory obligations,
- provide transparent calculations that can be inspected, reproduced, and audited.

Instead of adding another dashboard, the workbook productizes a repeatable inventory planning methodology that can be refreshed in minutes and understood by both operational users and technical reviewers.
