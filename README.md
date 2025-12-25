📊 Modern Data Table with TanStack Table v8
A lightweight, high-performance data table implementation using React, TanStack Table (v8), and CSS3. This project demonstrates how to handle headless table logic, custom column rendering, nested data access, and modern UI styling.

✨ Features
Headless Logic: Powered by TanStack Table for maximum flexibility.

Dynamic Serial Numbers: Automatic calculation of row indices.

Nested Data Mapping: Seamlessly rendering deep objects (e.g., address.city).

Modern UI: A clean, responsive design with hover states and polished typography.

Type-Safe Columns: Implemented using createColumnHelper.

🚀 Getting Started

1. Prerequisites
   Node.js (v16.x or higher)

npm or yarn

2. Installation
   Clone the repository and install the dependencies:

Bash

git clone https://github.com/your-username/tanstack-table-demo.git
cd tanstack-table-demo
npm install 3. Dependencies
The project relies on the following core package:

Bash

npm install @tanstack/react-table 4. Running the Project
Bash

npm run dev
📁 Project Structure
Plaintext

src/
├── components/
│ └── Table.jsx # Core table component logic
├── constants/
│ └── data.json # Sample JSON data (Name, Email, Address)
├── App.css # Modern table styling
└── App.jsx # Entry point
🛠️ Implementation Details
Column Configuration
The table uses createColumnHelper to define four distinct columns:

S.No: A display column calculating index + 1.

Name: Accessor for the name string.

Email: Accessor for the email string.

City: A nested accessor mapping address.city.

Styling Strategy
The table uses a Modern Card aesthetic:

border-spacing: 0 for clean internal lines.

overflow: hidden on the container to maintain rounded corners.

Subtle transitions on tbody tr:hover for improved UX.

📝 Sample Data Format
The table expects an array of objects structured as follows:

JSON

{
"id": 1,
"name": "Arjun Sharma",
"email": "arjun.sharma@example.com",
"address": {
"city": "Mumbai",
"street": "123 Marine Drive",
"zipcode": "400001"
}
}
