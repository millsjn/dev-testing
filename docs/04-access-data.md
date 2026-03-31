---
title: How to Access Data
description: Learn how to access the secure data you have been approved to access.
order: 4
lastUpdated: 2025-03-31
---

# How to Access Data

This section provides information on how to locate the secure data you’ve been approved to access in the ADRF.

> [!TIP]
> You can find a **video walkthrough** on how to find the sensitive data you’ve been approved to access in the ADRF in the `ADRF_Documentation` folder in the `G:' drive.

> [!NOTE] 
> **External Data and Code**: There is no direct method for uploading data or code from your system to the ADRF. Given the secure and protected environment provided by the ADRF, all code, data, and packages that are coming from outside of the ADRF must be carefully vetted to prevent leaks, disclosure, or unauthorized access. Your can submit a reqeust to import code or data to the ADRF by contacting `support@coleridgeinitiative.org`.

## Storage Locations

Sensitive data provided by data owners are stored in one of two locations in the ADRF:
1. **Unsctructured data storage** (`G:` Drive)
2. **Structured data storage** (AWS Redshift)

### Accessing data stored in unstructured data storage
Unstructured data, such as CSVs, Stata DTAs, SAS data, are stored in the “G” drive. Project teams will have read-only access to the data folders in this drive that they have been approved to access.

The G: Drive is located in the ADRF's file system. You can find it by going to the Folder icon in the Windows Task Bar.

### Accessing data stored in structured data storage
Structured data, or data that are stored in relational databases, are stored in AWS Redshift, an MPP platform that is built on SQL and is specifically designed to handle larger data assets. Users access structured data either through **DBeaver** – the ADRF's Database Access tool – or by porting directly to Redshift through their preferred **statistical package** (like R, or Python).

For detailed instructions on how to access data in structed data storage, please see the ADRF's [Redshift Querying Guide](/docs/advanced/redshift-querying-guide.md)


<br>

---
# Support & Navigation

**Need help?**
- Email: support@coleridgeinitiative.org
- Hours: Monday-Friday, 9 AM - 5 PM ET

**Navigation**
- ⬅️ [Back to Home](../README.md)

