# Entornos-7.5
EJERCICIO 1:
```mermaid
flowchart LR
 subgraph GymMaster_System["Booking Management System"]
        UC1("Login")
        UC2("Book Class")
        UC3("Join Waitlist")
        UC4("Manage Classes")
        UC5("Cancel Session")
  end
    UC2 -. |&lt;&lt;include&gt;&gt;| .- UC1
    UC3 -. |&lt;&lt;extend&gt;&gt;| .- UC2
    UC4 -. |&lt;&lt;include&gt;&gt;| .- UC1
    UC5 -. |&lt;&lt;include&gt;&gt;| .- UC1
    Member(("Member")) --> UC2
    Admin(("Administrator")) --> UC4 & UC5
```
