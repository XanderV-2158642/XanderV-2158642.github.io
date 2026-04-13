---
layout: page
title: "MotoValue"
description: "Second-hand motorcycle valuation platform"
technologies: ["Vercel", "Regression model"]
featured: true
date: 2025-01-01
---

# MotoValue

Second-hand Motorcycle Valuation Platform

## Overview

MotoValue allows users to input multiple motorcycles and receive a fair value price estimate. The price predictions are based on a regression model trained on bidding values from advertisements that disappeared shortly after the bid, indicating a successful sale at that price point.

## Key Factors

- **Age**: Year of manufacture/purchase
- **Kilometers**: Wear indicator (mileage)
- **Insurance**: Coverage history
- **Warranty**: Warranty status

## Features

### Catalog

List of all motorcycles you've added. A centralized inventory view showing all entered motorcycles with their basic details.

![Catalog](/assets/pictures/MotoValue/Catalog.png)

### Overview

Per-motorcycle detailed view showcasing the different costs and benefits each motorcycle has. Shows insurance, warranty status, and other factors that affect valuation.

![Overview](/assets/pictures/MotoValue/Overview.png)

### Market

Comparison view plotting fair value vs. listing price on a scatter plot. Helps visualize how each motorcycle compares to the market average.

![Market](/assets/pictures/MotoValue/Market.png)

## Tech Stack

- Vercel (Hosting)
- Regression model for price prediction

[View Project](https://moto-value.vercel.app)