```mermaid
erDiagram
    PERSON ||--o{ ENROLLMENT : registration
    SECTION ||--o{ ENROLLMENT : records

    Person {
         person_id PK
         first_name
         last_name
         birth_date
         gender
         address
         city
         state
         zip
    }

    SECTION {
         subject PK
         number PK
         section PK
         title
         credit_hours
         instructor
         days
         start_time
         end_time
    }

    ENROLLMENT {
         student_id PK
         subject FK
         FK
         section FK
    }
```


# project-2-week-3
