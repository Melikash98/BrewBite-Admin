# BrewBite-Admin
flowchart TB
    %% =========================
    %% BrewBite Admin Flowchart
    %% =========================

    subgraph A[Authentication Flow]
        A1[Admin opens login page]
        A2[Submit email / username + password]
        A3{Credentials valid?}
        A4[Authentication Failed]
        A5[Generate JWT Token]
        A6[Return token to client]
        A7[Access granted to protected resources]

        A1 --> A2 --> A3
        A3 -- No --> A4
        A3 -- Yes --> A5 --> A6 --> A7
    end

    subgraph B[Order Management Flow]
        B1[Customer places order]
        B2[Order sent to backend API]
        B3[Validate order data]
        B4{Order valid?}
        B5[Order Failed]
        B6[Save order in database]
        B7[Order confirmed]
        B8[Notify admin]
        B9[Admin views order]
        B10[Update order status]
        B11[Revenue, ratings, comments, complaints and analytics updated]

        B1 --> B2 --> B3 --> B4
        B4 -- No --> B5
        B4 -- Yes --> B6 --> B7 --> B8 --> B9 --> B10 --> B11
    end

    subgraph C[System Components]
        C1[Admin Web Panel]
        C2[Spring Security + JWT]
        C3[Spring Boot REST API]
        C4[Controllers]
        C5[Services]
        C6[Repositories]
        C7[Entities / Models]
        C8[(PostgreSQL)]
        C9[(Cloudinary)]
        C10[(Redis)]

        C1 --> C2 --> C3
        C3 --> C4 --> C5 --> C6 --> C7
        C6 --> C8
        C5 --> C9
        C5 --> C10
    end

    A7 --> C1
    B11 --> C1
