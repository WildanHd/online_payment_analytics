# digital_wallet_transactions

# Explore the online transaction data consist of Analytics Pipeline & Data Mart

An end-to-end local prototype simulating a transaction processing and business intelligence layer.
This repository models raw payment payload extractions, structures analytical Data Mart in PostgreSQL, and explain financial KPIs and system reliability metrics in Metabase.

## Architecture & Data Floe

[Raw Transaction Payloads] --- (Python ETL) --- [PostgreSQL Data Lake]
---> [SQL Mart 1: Financial economics (daily_transaction)]
---> [SQL Mart 2: Gateway & Acquirer Reliability (system_funnel)]
[Metabase Analytical Dashboard]

## Core Business & Operational Metrics Tracked

| Monitoring Metric | Primary KPIs | Derived Values |
| :--- | :--- | :--- |
| **Financial Health** | **GPV (Gross Payment Volume)**, **Take-Rate Revenue**, **Payment Mix Share** | Tracks net monetization spread across Cards, Wallets, and Alternative Payment Methods |
| **Conversion Funnel** | **Authorization Rate (%)**, **Soft vs. Hard Decline Breakdown** | Identifies merchant drop-offs and friction in checkout flows |
| **System Operations** | **$P_{50} / P_{95} / P_{99}$ API Latency (ms)**, **INtegration_Rail Stability** | Monitors infrastructure health across Plugin vs. Raw API traffic. |
