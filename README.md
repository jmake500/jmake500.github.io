# jmake500.github.io

flowchart TD
    A["User logs into OCC"] --> B["Navigates to Accounts > Invoices"]
    B --> C["Selects Pay Invoice"]
    C --> D["OCC pulls CyberSource form via API"]
    D --> E["User completes form"]
    E --> F[("Payment logged in CyberSource")]
    F --> G["Email to Restek Accounts Receivable"]
    F --> H["Confirmation email to client"]
    G --> I["AR looks up payment in CyberSource UI"]
    I --> J["AR manually enters payment in IFS"]
