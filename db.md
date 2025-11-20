erDiagram
  ROLES ||--o{ USERS : has
  BRANCHES ||--o{ USERS : contains
  USERS ||--o{ TEAM_MEMBERSHIP : leads
  USERS ||--o{ TEAM_MEMBERSHIP : member_of
  POLICIES ||--o{ INVOICES : referenced_by
  BRANCHES ||--o{ INVOICES : issues
  USERS ||--o{ INVOICES : cashier_processed
  USERS ||--o{ PROMOTIONS : subject
  ROLES ||--o{ PROMOTIONS : role_from
  ROLES ||--o{ PROMOTIONS : role_to
  MONTHLY_TARGETS ||--o{ USERS : target_for
