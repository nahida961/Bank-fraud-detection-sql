# 🏦 Bank Fraud Detection & Customer Risk Analytics

![SQL](https://img.shields.io/badge/SQL-Advanced-blue) ![Domain](https://img.shields.io/badge/Domain-Banking%20%2F%20FinTech-navy) ![Status](https://img.shields.io/badge/Status-Complete-green)

## Overview
A simulated relational banking database designed to detect fraudulent transactions, flag AML (Anti-Money Laundering) risk, and segment customers by financial profile. Built to demonstrate real-world financial data engineering skills.

---

## Problem Statement
Banks process millions of transactions daily. Manual review is impossible. This project automates:
- Detection of suspicious transactions using pattern-based SQL logic
- Daily compliance reporting for AML teams
- Customer segmentation for risk profiling and marketing

---

## Database Schema

| Table | Description |
|-------|-------------|
| `Customers` | Customer details, account creation date, KYC Risk Tier (Low / Medium / High) |
| `Accounts` | Account number, balance, account type (Checking / Savings), status |
| `Transactions` | Transaction ID, timestamp, amount, location, channel (ATM / Online / Branch), status |

---

## Key Features

### 1. Fraud Detection (Window Functions)
Used `PARTITION BY` window functions to flag:
- Transactions exceeding $10,000
- Accounts with 3+ distinct international transactions within a 1-hour window

### 2. AML Compliance Reporting (Stored Procedures & Views)
Created automated Views and Stored Procedures to generate daily High-Risk Transaction reports — reducing manual compliance workload.

### 3. Customer Segmentation (CASE WHEN)
Applied CASE WHEN logic across 10,000+ records to categorize accounts into:
- 🔴 Under-funded | 🟡 Standard | 🟢 High-Net-Worth

---

## SQL Concepts Used
`Window Functions` · `PARTITION BY` · `CASE WHEN` · `Stored Procedures` · `Views` · `Joins` · `Subqueries` · `Aggregate Functions`

---

## Relevance to Industry
This project simulates a real bank's AML compliance pipeline. The schema, logic, and reporting structure mirror what financial institutions use to meet regulatory requirements (RBI / SEBI / FATF guidelines).

---

## Author
**Nahida Banoo** — BSc (Hons) Computer Science, University of Delhi  
Research: Financial Fraud Detection (Conference Paper, 2024)
