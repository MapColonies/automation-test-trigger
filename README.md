Certainly! Here's the updated README file with the additional information:

---

# Automation Tests Trigger README

This HELM file triggers the export ingestion and update tests sequentially in a QA environment.

## Setup Instructions

1. **Clone the Project:**
   ```
   git clone https://github.com/MapColonies/automation-test-trigger.git
   ```
   Clone the project repository to your local environment.

2. **Install the Trigger:**
   ```
   helm install automation-tests-job
   ```
   Install the trigger named `automation-tests-job` in the QA environment.

   **Note:** Ensure to keep the RELEASE name because the ROUTE for CALLBACK is configured based on it. The values are encapsulated in PVC.

## Running Tests

Once installed, the tests will run automatically one after the other. If one of the tests gets stuck, the subsequent tests will not run until the issue is resolved.

You can monitor the results through the POD named `EXPORT-MERGER`.

To view the logs:
```
cd /layerSources/automation/logs
```

---

