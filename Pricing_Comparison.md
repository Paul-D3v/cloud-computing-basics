# Cloud Pricing Comparison Across Regions

## Introduction

Cloud providers charge different prices for the same services in different geographic regions. This guide shows you how to compare pricing and includes actual price comparisons for common services.

---

## Why Prices Vary by Region

### Factors Affecting Regional Pricing:

1. **Data Center Costs**
   - Real estate prices
   - Construction costs
   - Local regulations

2. **Energy Costs**
   - Electricity prices vary by region
   - Cooling requirements (climate)

3. **Network Costs**
   - Internet bandwidth costs
   - Peering agreements
   - Connectivity infrastructure

4. **Demand and Competition**
   - High-demand regions may have higher prices
   - Newer regions may have promotional pricing

5. **Local Taxes and Regulations**
   - Import duties on hardware
   - Data privacy laws
   - Environmental regulations

---

## AWS Pricing Calculator

### How to Use AWS Pricing Calculator:

**Step 1: Access the Calculator**
- Visit: https://calculator.aws
- Click **"Create estimate"**

**Step 2: Add Services**
- Click **"Add service"**
- Search for service (e.g., "EC2", "S3", "RDS")
- Click **"Configure"**

**Step 3: Configure Service (Example: EC2)**
```
Description: Web Server Instance
Region: US East (N. Virginia) [or select different region]
Quick estimate or Advanced estimate: Quick estimate

Instance details:
- Operating System: Linux
- Instance type: t3.micro
- Workload: Daily (specify hours)
- Storage: 30 GB General Purpose SSD (gp3)
```
- Click **"Save and add service"**

**Step 4: Change Region for Comparison**
- At the top, click **"Region: US East (N. Virginia)"**
- Select different region (e.g., "EU (Frankfurt)")
- Notice price changes automatically

**Step 5: Export or Save**
- Click **"View summary"**
- Click **"Export"** to save as CSV or PDF
- Take screenshots for documentation

---

## AWS Regional Pricing Comparison

### EC2 Instance Pricing (t3.micro - 1 month, 730 hours)

| Region | Region Code | Price/Hour | Monthly Cost | vs US East |
|--------|-------------|------------|--------------|------------|
| **US East (N. Virginia)** | us-east-1 | $0.0104 | **$7.59** | Baseline |
| **US West (Oregon)** | us-west-2 | $0.0104 | $7.59 | Same |
| **US West (N. California)** | us-west-1 | $0.0117 | $8.54 | +12.5% |
| **Canada (Central)** | ca-central-1 | $0.0116 | $8.47 | +11.6% |
| **EU (Ireland)** | eu-west-1 | $0.0104 | $7.59 | Same |
| **EU (Frankfurt)** | eu-central-1 | $0.0117 | $8.54 | +12.5% |
| **EU (London)** | eu-west-2 | $0.0114 | $8.32 | +9.6% |
| **EU (Paris)** | eu-west-3 | $0.0114 | $8.32 | +9.6% |
| **Asia Pacific (Tokyo)** | ap-northeast-1 | $0.0130 | $9.49 | +25.0% |
| **Asia Pacific (Singapore)** | ap-southeast-1 | $0.0122 | $8.91 | +17.4% |
| **Asia Pacific (Sydney)** | ap-southeast-2 | $0.0130 | $9.49 | +25.0% |
| **Asia Pacific (Mumbai)** | ap-south-1 | $0.0104 | $7.59 | Same |
| **South America (São Paulo)** | sa-east-1 | $0.0156 | $11.39 | +50.0% |

**Key Insights:**
- 🟢 **Cheapest**: US East, US West Oregon, EU Ireland, Mumbai
- 🔴 **Most Expensive**: São Paulo (50% premium)
- 📊 **Average increase**: 10-25% for most regions
- ⚡ **Best value for US**: US East (N. Virginia)
- ⚡ **Best value for EU**: EU (Ireland)

---

### S3 Storage Pricing (100 GB for 1 month)

| Region | Standard Storage | Data Transfer Out | Total Monthly |
|--------|------------------|-------------------|---------------|
| **US East (N. Virginia)** | $2.30 | $0.90/GB | **$92.30** (100GB transfer) |
| **US West (Oregon)** | $2.30 | $0.90/GB | $92.30 |
| **EU (Ireland)** | $2.30 | $0.90/GB | $92.30 |
| **EU (Frankfurt)** | $2.47 | $0.90/GB | $92.47 |
| **Asia Pacific (Tokyo)** | $2.55 | $1.14/GB | $116.55 |
| **Asia Pacific (Singapore)** | $2.50 | $1.20/GB | $122.50 |
| **South America (São Paulo)** | $3.40 | $1.50/GB | $153.40 |

**Key Insights:**
- Storage costs are relatively consistent (within 10%)
- Data transfer costs vary significantly (up to 67% more)
- Asia Pacific and South America have higher egress charges

---

### RDS Database Pricing (MySQL db.t3.micro - 1 month)

| Region | Price/Hour | Monthly Cost | Storage (20GB) | Total |
|--------|------------|--------------|----------------|-------|
| **US East (N. Virginia)** | $0.017 | $12.41 | $2.30 | **$14.71** |
| **US West (Oregon)** | $0.017 | $12.41 | $2.30 | $14.71 |
| **EU (Ireland)** | $0.018 | $13.14 | $2.53 | $15.67 |
| **EU (Frankfurt)** | $0.020 | $14.60 | $2.76 | $17.36 |
| **Asia Pacific (Tokyo)** | $0.023 | $16.79 | $2.76 | $19.55 |
| **Asia Pacific (Singapore)** | $0.022 | $16.06 | $2.76 | $18.82 |
| **South America (São Paulo)** | $0.030 | $21.90 | $3.68 | $25.58 |

---

## Google Cloud Platform (GCP) Pricing

### How to Use GCP Pricing Calculator:

**Step 1: Access the Calculator**
- Visit: https://cloud.google.com/products/calculator
- Click **"Add to estimate"**

**Step 2: Select Service**
- Choose service (e.g., "Compute Engine", "Cloud Storage")
- Click service to configure

**Step 3: Configure (Example: Compute Engine)**
```
Location: Iowa (us-central1) [or select different region]

Instance details:
- Machine family: General-purpose
- Series: E2
- Machine type: e2-micro
- Number of instances: 1
- Operating System: Free (Debian, CentOS, Ubuntu)
- Provisioning model: Regular
- Usage: 730 hours/month

Persistent Disk:
- Type: Standard
- Size: 30 GB
```
- Configuration shows monthly cost

**Step 4: Change Region**
- Click on region dropdown
- Select different region
- Cost updates automatically

**Step 5: Save Estimate**
- Click **"Save estimate"**
- Click **"Share"** to get URL
- Take screenshots

---

## GCP Regional Pricing Comparison

### Compute Engine Pricing (e2-micro - 1 month, 730 hours)

| Region | Region Code | Price/Hour | Monthly Cost | vs Iowa |
|--------|-------------|------------|--------------|---------|
| **Iowa** | us-central1 | $0.007614 | **$5.56** | Baseline |
| **Oregon** | us-west1 | $0.007614 | $5.56 | Same |
| **South Carolina** | us-east1 | $0.007614 | $5.56 | Same |
| **N. Virginia** | us-east4 | $0.008583 | $6.27 | +12.7% |
| **Belgium** | europe-west1 | $0.008397 | $6.13 | +10.3% |
| **London** | europe-west2 | $0.009302 | $6.79 | +22.1% |
| **Frankfurt** | europe-west3 | $0.009302 | $6.79 | +22.1% |
| **Tokyo** | asia-northeast1 | $0.009857 | $7.20 | +29.5% |
| **Singapore** | asia-southeast1 | $0.008956 | $6.54 | +17.6% |
| **Sydney** | australia-southeast1 | $0.010671 | $7.79 | +40.1% |
| **São Paulo** | southamerica-east1 | $0.012048 | $8.80 | +58.3% |

**Key Insights:**
- 🟢 **Cheapest**: US regions (Iowa, Oregon, South Carolina)
- 🔴 **Most Expensive**: São Paulo (58% premium)
- 📊 **Europe**: 10-22% more than US
- 📊 **Asia Pacific**: 18-40% more than US

---

### Cloud Storage Pricing (100 GB Standard Storage)

| Region | Storage/GB/Month | 100GB Monthly | Data Egress (per GB) |
|--------|------------------|---------------|---------------------|
| **Iowa (us-central1)** | $0.020 | **$2.00** | $0.12 |
| **Belgium (europe-west1)** | $0.020 | $2.00 | $0.12 |
| **London (europe-west2)** | $0.023 | $2.30 | $0.12 |
| **Tokyo (asia-northeast1)** | $0.023 | $2.30 | $0.14 |
| **Singapore (asia-southeast1)** | $0.023 | $2.30 | $0.14 |
| **Sydney (australia-southeast1)** | $0.023 | $2.30 | $0.19 |

---

## Microsoft Azure Pricing

### How to Use Azure Pricing Calculator:

**Step 1: Access the Calculator**
- Visit: https://azure.microsoft.com/pricing/calculator
- Services are organized by category

**Step 2: Select Service**
- Scroll or search for service
- Click **"+"** next to service (e.g., "Virtual Machines")

**Step 3: Configure (Example: Virtual Machines)**
```
Region: East US [or select different region]

Virtual Machine:
- Operating System: Linux
- Type: (Basic)
- Tier: Standard
- Instance: B1S (1 vCPU, 1 GB RAM)
- Virtual machines: 1
- Running time: 730 Hours/Month

Managed Disks:
- Storage: S4 (32 GB)
- Disk: 1
```
- View estimated monthly cost

**Step 4: Change Region**
- Change region in dropdown
- Cost updates automatically

**Step 5: Export**
- Click **"Export"** to download estimate
- Take screenshots
- Click **"Share"** to get URL

---

## Azure Regional Pricing Comparison

### Virtual Machine Pricing (B1S - 1 vCPU, 1GB RAM - 730 hours/month)

| Region | Monthly Cost | Storage (32GB) | Total | vs East US |
|--------|--------------|----------------|-------|------------|
| **East US** | $7.59 | $1.54 | **$9.13** | Baseline |
| **East US 2** | $7.59 | $1.54 | $9.13 | Same |
| **West US** | $7.59 | $1.54 | $9.13 | Same |
| **West US 2** | $7.59 | $1.54 | $9.13 | Same |
| **Central US** | $7.59 | $1.54 | $9.13 | Same |
| **North Europe** | $8.26 | $1.68 | $9.94 | +8.9% |
| **West Europe** | $8.62 | $1.75 | $10.37 | +13.6% |
| **UK South** | $8.91 | $1.81 | $10.72 | +17.4% |
| **Japan East** | $9.72 | $1.98 | $11.70 | +28.1% |
| **Japan West** | $10.69 | $2.17 | $12.86 | +40.9% |
| **Southeast Asia** | $9.28 | $1.89 | $11.17 | +22.3% |
| **Australia East** | $9.87 | $2.01 | $11.88 | +30.1% |
| **Brazil South** | $11.39 | $2.32 | $13.71 | +50.2% |

**Key Insights:**
- 🟢 **Cheapest**: All US regions (same price)
- 🔴 **Most Expensive**: Brazil South (50% premium)
- 📊 **Europe**: 9-17% more than US
- 📊 **Asia Pacific**: 22-41% more than US

---

### Blob Storage Pricing (100 GB Hot Tier)

| Region | Storage (per GB) | 100GB Monthly | Bandwidth Out (per GB) |
|--------|------------------|---------------|------------------------|
| **East US** | $0.0184 | **$1.84** | $0.0875 |
| **West Europe** | $0.0202 | $2.02 | $0.0875 |
| **UK South** | $0.0210 | $2.10 | $0.0875 |
| **Japan East** | $0.0212 | $2.12 | $0.1100 |
| **Southeast Asia** | $0.0205 | $2.05 | $0.1200 |
| **Australia East** | $0.0215 | $2.15 | $0.1381 |
| **Brazil South** | $0.0276 | $2.76 | $0.1813 |

---

## Cross-Provider Regional Comparison

### Virtual Machine (Small Instance - 1 vCPU, ~1GB RAM, 730 hours/month)

| Provider | US East | EU West | Asia Pacific | South America |
|----------|---------|---------|--------------|---------------|
| **AWS** (t3.micro) | $7.59 | $7.59-8.54 | $8.91-9.49 | $11.39 |
| **GCP** (e2-micro) | $5.56 | $6.13-6.79 | $6.54-7.79 | $8.80 |
| **Azure** (B1S) | $9.13 | $9.94-10.72 | $11.17-11.88 | $13.71 |

**Winner by Region:**
- 🥇 **US East**: GCP ($5.56)
- 🥇 **EU West**: GCP ($6.13-6.79)
- 🥇 **Asia Pacific**: GCP ($6.54-7.79)
- 🥇 **South America**: GCP ($8.80)

---

### Object Storage (100 GB storage, 100 GB transfer out)

| Provider | US East | EU West | Asia Pacific | South America |
|----------|---------|---------|--------------|---------------|
| **AWS S3** | $92.30 | $92.30-92.47 | $116.55-122.50 | $153.40 |
| **GCP Cloud Storage** | $14.00 | $14.00 | $16.00-21.00 | ~$20.00 |
| **Azure Blob** | $10.59 | $11.77-12.85 | $14.17-15.65 | $20.89 |

**Winner by Region:**
- 🥇 **US East**: Azure ($10.59)
- 🥇 **EU West**: Azure ($11.77-12.85)
- 🥇 **Asia Pacific**: GCP ($16.00-21.00)
- 🥇 **South America**: GCP (~$20.00)

---

## Key Findings

### 1. Regional Price Variations
- **US Regions**: Generally cheapest (baseline)
- **Europe**: 10-20% more expensive
- **Asia Pacific**: 20-40% more expensive
- **South America**: 50-60% more expensive

### 2. Most Expensive Regions (Consistently)
1. **Brazil (São Paulo)**: +50-60%
2. **Australia (Sydney)**: +30-40%
3. **Japan (Tokyo/Osaka)**: +25-40%

### 3. Best Value Regions
1. **US Central/East**: Cheapest overall
2. **EU Ireland**: Best value in Europe
3. **Asia Mumbai**: Best value in Asia

### 4. Provider Comparison
- **GCP**: Generally cheapest for compute
- **Azure**: Competitive for storage
- **AWS**: Mid-range, most regions available

---

## Factors to Consider When Choosing Regions

### 1. **Latency**
- Choose regions closest to your users
- Latency matters more than small price differences
- Use CDN to serve global users

### 2. **Data Residency**
- Legal requirements (GDPR, data sovereignty)
- Industry regulations (HIPAA, PCI-DSS)
- Customer preferences

### 3. **Availability**
- Not all services available in all regions
- Some regions have better SLAs
- Consider multi-region for high availability

### 4. **Cost vs. Performance**
- Sometimes cheaper regions have older hardware
- Newer regions may have better performance
- Balance cost savings with performance needs

### 5. **Data Transfer Costs**
- Egress (outbound) charges vary significantly
- Inter-region transfer can be expensive
- Consider traffic patterns

---

## How to Take Screenshots for Assignment

### What to Capture:

1. **Pricing Calculator Page**
   - Full screen showing service configuration
   - Highlighted region selector
   - Visible monthly cost estimate

2. **Price Comparison Table**
   - Multiple regions shown side-by-side
   - Clear price differences
   - Date visible

3. **Regional Map** (if available)
   - Visual representation of regions
   - Price overlay

4. **Export/Summary**
   - Final cost estimate
   - Breakdown of charges

### Screenshot Tips:

**Windows:**
- Press `Windows + Shift + S` for Snipping Tool
- Select area to capture
- Save as PNG

**Mac:**
- Press `Cmd + Shift + 4`
- Drag to select area
- Image saves to Desktop

**Full Page Screenshot:**
- Use browser extension (Awesome Screenshot, Full Page Screen Capture)
- Captures entire scrollable page

**Organize Screenshots:**
```
screenshots/
├── aws-pricing-us-east.png
├── aws-pricing-eu-west.png
├── aws-pricing-asia.png
├── gcp-pricing-us.png
├── gcp-pricing-eu.png
├── azure-pricing-us.png
└── pricing-comparison-table.png
```

---

## Conclusion

Regional pricing varies significantly across cloud providers:
- ✅ US regions offer best value
- ✅ Europe costs 10-20% more
- ✅ Asia and South America can cost 50%+ more
- ✅ GCP generally cheapest for compute
- ✅ Storage pricing more consistent across regions

**Recommendation**: Start with closest region to users, then optimize for cost if budget-sensitive.

---

## Resources

**AWS Pricing Calculator**: https://calculator.aws  
**GCP Pricing Calculator**: https://cloud.google.com/products/calculator  
**Azure Pricing Calculator**: https://azure.microsoft.com/pricing/calculator

**AWS Regions**: https://aws.amazon.com/about-aws/global-infrastructure/regions_az  
**GCP Regions**: https://cloud.google.com/about/locations  
**Azure Regions**: https://azure.microsoft.com/global-infrastructure/geographies
