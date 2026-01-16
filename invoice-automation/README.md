# 📊 Invoice Automation System with AI Extraction

**Template for deploying AI-powered invoice processing for small businesses**

---

## 🎯 What This Does

Automatically processes invoices across multiple email accounts:
- ✅ Scans Gmail for invoice attachments
- ✅ Extracts data with Google Cloud Vision API (amount, invoice #, IBAN)
- ✅ Organizes in Google Drive (year/quarter folders)
- ✅ Tracks in spreadsheets with auto-filled data
- ✅ Runs Q1+Q2 historical scan on first execution
- ✅ **Cost: FREE** (within 1,000 Vision API calls/month)

---

## 📈 Results

- **98% automation** (manual: category + notes only)
- **80% time savings** (2 min → 15 sec per invoice)
- **€0/month cost** (free tier sufficient for most businesses)
- **90%+ accuracy** (Vision API extraction)

---

## 👥 Perfect For

- Small businesses with 50-500 invoices/month
- Teams using Google Workspace
- Companies wanting to eliminate manual data entry
- Organizations needing organized invoice archives

---

## ⚙️ Quick Start

### 1. Prerequisites
- Google Workspace account (business email)
- 30 minutes for setup
- No coding required

### 2. Setup (Follow DEPLOYMENT_GUIDE.md)
1. Enable Google Cloud APIs (5 min)
2. Configure OAuth consent (3 min)
3. Deploy code to Apps Script (7 min)
4. Authorize permissions (2 min)
5. Test & verify (5 min)

### 3. Customize Configuration
Edit `CONFIG` object in code:
```javascript
const CONFIG = {
  emailAccounts: ['info@yourcompany.com', 'admin@yourcompany.com'],
  mainFolderName: 'INVOICES_FACTURAS_COMPANY',
  shareWithUsers: ['manager@yourcompany.com'],
  historicalScanStartDate: '2025-01-01',  // Change for your needs
  historicalScanEndDate: '2025-06-30'      // Change for your needs
};
```

---

## 📁 Files Included

- **INVOICE_AUTOMATION_FINAL.gs** - Complete production code
- **DEPLOYMENT_GUIDE.md** - Step-by-step setup instructions
- **CONFIGURATION_TEMPLATE.md** - How to customize for clients
- **TROUBLESHOOTING.md** - Common issues & fixes
- **IMPLEMENTATION_LOG.md** - Lessons learned from real deployment

---

## 🔧 Features

### Core Features:
- Multi-account email monitoring
- Google Cloud Vision API integration
- Automatic folder/spreadsheet creation
- Duplicate detection
- Team collaboration (shared folders)
- Email notifications
- Error handling & logging

### Advanced Features:
- **Auto Historical Scan:** Imports Q1+Q2 on first run
- **Custom date ranges:** Configurable historical periods
- **Multi-currency support:** EUR, USD, GBP
- **Flexible keywords:** Customize invoice detection
- **Manual overrides:** Run scans on-demand

---

## 💰 Cost Analysis

**Free Tier (Sufficient for most businesses):**
- Google Apps Script: FREE
- Gmail API: FREE
- Drive API: FREE
- Sheets API: FREE
- Vision API: 1,000 requests/month FREE

**Your Likely Usage:**
- 100-300 invoices/month = FREE
- 500 invoices/month = FREE
- 1,000+ invoices/month = ~€1.50/1,000 extra

**ROI:**
- Setup time: 30 min
- Monthly savings: 100-300 minutes (admin time)
- Break-even: Immediate
- Ongoing value: Priceless (eliminates repetitive work)

---

## 🚀 Deployment Checklist

- [ ] Read DEPLOYMENT_GUIDE.md
- [ ] Create Google Cloud project
- [ ] Enable all 4 APIs (Vision, Drive, Gmail, Sheets)
- [ ] Set up OAuth consent
- [ ] Deploy code to Apps Script
- [ ] Customize CONFIG for client
- [ ] Run initial authorization
- [ ] Test with sample invoice
- [ ] Verify historical scan worked
- [ ] Set up daily triggers (3x daily)
- [ ] Document for client handoff

---

## 📊 Client Success Story

**Teatro Metamorfosis** (Barcelona cultural venue)
- **Challenge:** 300 invoices/month across 3 email accounts
- **Solution:** Deployed this template (customized)
- **Results:** 
  - 98% automation achieved
  - 225 min/month saved
  - €0 monthly cost
  - Team loves it!

Full case study: See `CASE_STUDY_Teatro.html`

---

## 🛠️ Customization Guide

### For Different Industries:
- **Restaurants:** Change keywords to include "delivery", "supplier"
- **Property Management:** Add "maintenance", "repair"
- **Freelancers:** Configure for client payments
- **Non-profits:** Track donation receipts

### Language Support:
Edit `invoiceKeywords` and `quarters` in CONFIG

### Folder Structure:
Modify `quarters` array for monthly/weekly organization

---

## 🐛 Troubleshooting

**Common Issues:**
1. **"Server error"** → Wait 30-60 min after enabling APIs
2. **"Can't create folder"** → Enable Drive API in GCP
3. **"OAuth required"** → Set up consent screen first
4. **Vision API extraction fails** → Normal for 5-10% of invoices

See TROUBLESHOOTING.md for complete guide.

---

## 📚 Documentation

- **DEPLOYMENT_GUIDE.md** - Setup instructions
- **CONFIGURATION_TEMPLATE.md** - Customization options
- **TROUBLESHOOTING.md** - Error resolution
- **IMPLEMENTATION_LOG.md** - Lessons from real deployment
- **API_REFERENCE.md** - Function documentation

---

## 🤝 Support

**For implementation help:**
- Read DEPLOYMENT_GUIDE.md first
- Check TROUBLESHOOTING.md for common issues
- Review IMPLEMENTATION_LOG.md for lessons learned

**For customization:**
- See CONFIGURATION_TEMPLATE.md
- Edit CONFIG object in code
- Test with small batch first

---

## 📝 License

Template for commercial use in client implementations.  
Credit: Sarah Poer / Mother of Chaos AI Solutions

---

## 🎓 Learn More

**Technologies Used:**
- Google Apps Script (automation)
- Google Cloud Vision API (OCR/extraction)
- Gmail API (email processing)
- Drive API (file storage)
- Sheets API (data tracking)

**Skills Demonstrated:**
- AI/ML integration
- Business process automation
- Google Workspace development
- Invoice processing workflows
- Client solution deployment

---

**Ready to deploy? Start with DEPLOYMENT_GUIDE.md →**
