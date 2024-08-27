## Service Desk
### **Overview**

The Company manages a large-scale infrastructure of weather-measuring equipment hosted on single-board computers globally. They require a custom Service Desk solution to manage support tickets and incidents, prioritizing quality and efficiency in incident response. The solution should automate the issue lifecycle and allow engineers and managers to handle incidents effectively.
### Functional Requirements (FR)

- **[FR-010]** Every issue in the infrastructure should trigger an alert to the engineers on duty.
    - **[FR-011]** Issues are passed to the system via Prometheus Alert Manager.
    - **[FR-012]** Alerts should include essential information like issue location and equipment type.
    - **[FR-013]** Engineers should be able to acknowledge and take ownership of incidents directly from the alert.
    - **[FR-014]** Issues can be created by a Customer using form on the system website. In that case issue is closed only by the Customer who opened it.
- **[FR-020]** Issues should be classified by severity automatically when possible, with the option for engineers to manually adjust the severity.
    - **[FR-022] **Engineers get monetary bonuses based on their performance. Money should be accumulated on their Account and payed out every month.
    - **[FR-025]** Managers can validate and override severity classifications (Cursed).

- **[FR-030]** Managers can generate basic reports on the cost of support operations, categorized by the number of issues and severity levels.
    - **[FR-031]** Engineers’ performance should be tracked based on their response and resolution times.
- **[FR-070]** If an Engineer on duty does not respond to an incident within the designated time, they should receive a phone call from the "Iron Lady," an automated external notification service.
    - **[FR-071]** If the Engineer still does not respond, the alert escalates to the next Engineer on the duty queue.
    - **[FR-072]** Engineers are fined for not responding in time from their Account.

- **[FR-040]** Managers should be able to manage engineering duty schedules, ensuring regional coverage.
    - **[FR-041]** Engineers can only be assigned to regions where they are located.
- **[FR-050]** Managers should be able to hire new engineers and assign them to regions based on their location.


### Additional comments from the customer
- Alerts should be timely; every minute counts.
- The system must be scalable to accommodate growth in the number of incidents and users. We expect a maximum of 100 issues with our systems per day. Our developers are REALLY good, and the systems should not break more often than that.
- The system should be user-friendly. New engineers should not need to spend much time understanding the UI.
- Engineers should not be able to hack into managers' accounts and override severities to increase payouts.
- We have many competitors in the industry because we are highly successful.
