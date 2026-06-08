```mermaid
erDiagram
    PERSON ||--o{ ENROLLMENT : registration
    SECTION ||--o{ ENROLLMENT : records

    PERSON { <br/>
         PERSON_id PK <br/>
         first_name <br/>
         last_name<br/>
         birth_date <br/>
         gender <br/>
         address <br/>
         city <br/>
         state <br/>
         zip <br/>
    }

    SECTION { <br/>
         subject PK <br/>
         number PK <br/>
         section PK <br/>
         title <br/>
         credit_hours <br/>
         instructor <br/>
         days <br/>
         start_time <br/>
         end_time <br/>
    }

    ENROLLMENT { <br/>
         student_id PK <br/>
         subject FK <br/>
         number FK <br/>
         section FK <br/>
    } 
```


# project-2-week-3
