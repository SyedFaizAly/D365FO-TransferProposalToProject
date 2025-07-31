# 🚀 Transfer Proposal to Project – Dynamics 365 Finance & Operations

This powerful customization in **D365 F&O (Project Management & Accounting)** transforms the traditional, multi-step process of setting up projects from **Project Quotations** into a seamless **one-click automation**.

---

## 🌟 Key Highlights

✅ **Auto-generate Proposal IDs** using custom Number Sequence  
✅ **Enhanced Project Quotation Form** with new actionable buttons  
✅ **Dynamic Parameters** for automation control  
✅ **One-click Transfer to Project** — from Proposal to Forecast  
✅ **Complete Project Hierarchy Creation** in seconds

---

## 🧩 Core Features

### 1️⃣ **Automated Proposal ID Generation**
- Custom Number Sequence created for Proposal IDs.
- Automatically assigned during new Project Quotation creation.
- Implemented via **Form Extensions**, **CoC**, and custom logic.

### 2️⃣ **Custom Buttons on Project Quotation Form**
- **New Proposal**: Opens a new Project Quotation with a generated Proposal ID.
- **Add Quotation**: Opens form for adding a quotation to an existing Proposal ID.
- Buttons are context-aware, appearing based on conditions.

### 3️⃣ **Parameter-Driven Automation**
- Added custom fields to the **Project Management and Accounting Parameters** form.
- Used to control and influence the automation logic dynamically.

### 4️⃣ **Transfer Proposal to Project – Main Automation**
When the **Transfer** button is clicked:
- 🔍 Retrieves all Project Quotations with the same Proposal ID.
- 📄 Creates the **Project Contract**.
- 🏗️ Creates the **Project Header**.
- 🌿 Creates **Sub-Projects** for each quotation.
- 📦 Creates **Item Requirements** and **Forecasts** for each Sub-Project, based on Project Quotation Lines.

---

## 🧠 Business Value

> ✨ "This solution reduces hours of project setup effort, multiple decisions, and risk of human error into a single intelligent click — enabling smoother project delivery from quotation to execution." ✨

---

## 📁 Repo Structure


## 📦 Visual Studio Project Structure

All development was done using Visual Studio and D365 F&O development tools.

```plaintext
/TransferProposalToProject/
│
├── /Project/
│   ├── Classes/              # Automation logic
│   ├── FormExtensions/       # UI customizations and buttons
│   ├── TableExtensions/      # Custom fields and parameters
│   └── NumberSequence/       # Custom Proposal ID sequence
│   └── Base enums and EDTs/  # For fields
│   └── Label file/           # Labels to display in multiple language
│
├── /Screenshots/
│   ├── Proposal Buttons.png
│   ├── NewProposal.png
│   ├── AddQuotation.png
│   ├── ProjectQuotations.png
│   ├── ProjectHeaders.png
│   ├── ProjectContracts.png
│   ├── ProjectHeaders.png
│   ├── SubProject.png
│
└── README.md
