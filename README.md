```mermaid
graph TD
    A[User visits Application] --> B{Is user registered?}
    B -- No --> C[Register Account]
    B -- Yes --> D[Login]

    D --> E{User Role}
    E -- Student --> F[Browse Courses]
    F --> G[View Course Details]
    G --> H{Purchase Course?}
    H -- Yes --> I[Proceed to Payment]
    I --> J[Access Course Content]
    J --> K[Track Progress]
    K --> L[Complete Course & Get Certificate]

    E -- Instructor --> M[Create Course]
    M --> N[Upload Content (Videos, PDFs, Quizzes)]
    N --> O[Submit for Review]
    O --> P[Course Approved?]
    P -- Yes --> Q[Course Published]
    Q --> R[Student Enrollments]

    E -- Admin --> S[Review New Courses]
    S --> T[Approve/Reject Course]
    T --> U[Manage Users & Reports]

    style A fill:#f9f,stroke:#333,stroke-width:2px
    style E fill:#ccf,stroke:#333
 ...

