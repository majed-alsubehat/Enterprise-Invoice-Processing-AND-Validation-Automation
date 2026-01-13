Enterprise Invoice Processing & Validation Automation (RPA)

📌 Overview

This project is a training-focused Enterprise RPA automation built using UiPath.
It simulates a real-world invoice processing workflow without using any sensitive or real business data.

The automation reads invoice files from Excel, extracts invoice details, validates vendors and financial rules, applies decision logic, stores results, and generates a final summary report.


🎯 Project Objectives

-Simulate real enterprise invoice processing scenarios
-Apply structured RPA design (modular workflows)
-Practice data extraction, validation, and decision logic
-Generate structured outputs and summary reports
-Follow best practices suitable for GitHub portfolios


🗂 Project Structure
Enterprise-Invoice-Processing/
│
├── Invoices_Input/            # Sample invoice Excel files
├── VendorMaster/              # Vendor master data (Approved / Not Approved)
│
├── ReadInvoice.xaml           
├── ExtractInvoiceData.xaml    
├── ValidateInvoice.xaml       
├── DecisionEngine.xaml 
├── SaveResult.xaml            
├── Main.xaml                  
│
├── Approved_Invoices.xlsx
├── Rejected_Invoices.xlsx
├── Review_Invoices.xlsx
├── Final_Report.xlsx
│
└── README.md


🔄 Process Flow

1.Read Vendor Master data
2.Loop through invoice files (For Each File in Folder)
3.Read invoice data from Excel
4.Extract invoice fields (Invoice Number, Vendor, Amount, Tax, Total)
5.Validate business rules:
-Amount must be valid
-Total = Amount + Tax
-Vendor must be approved
6.Apply decision logic:
-Approved
-Rejected
-Needs Review
7.Save results into separate Excel files
8.Generate final summary report


📊 Validation Rules

-Amount ≥ 0
-Total must equal Amount + Tax
-Vendor must exist in Vendor Master
-Vendor status must be Approved

📈 Final Report

The automation generates a summary report including:
-Number of approved invoices
-Number of rejected invoices
-Number of invoices requiring review


🛠 Technologies Used
-UiPath Studio
-Excel Workbook Activities
-DataTables
