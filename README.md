```mermaid
erDiagram
    PERSON ||--o{ ENROLLMENT : registration
    SECTION ||--o{ ENROLLMENT : records

    PERSON {
        field person_id PK
        field first_name
        field last_name
        field birth_date
        field gender
        field address
        field city
        field state
        field zip
    }

    SECTION {
        field subject PK
        field number PK
        field section PK
        field title
        field credit_hours
        field instructor
        field days
        field start_time
        field end_time
    }

    ENROLLMENT {
        field student_id PK
        field subject PK
        field number PK
        field section PK
    }
```
