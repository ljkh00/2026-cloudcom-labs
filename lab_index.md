# Lab File Index

> **Subfolder structure adopted (Phase 0 decision).**
> All files below move to `weekNN/` subfolders before the first Git push.
> New paths listed in the rightmost column. Flat filenames kept here for backward reference during the transition.

| File (flat / current)                           | Toggle pattern                  | copyCode stopProp | expandAll | GHP meta | Status     | New path (subfolder)                                                                                              |
|-------------------------------------------------|---------------------------------|-------------------|-----------|----------|------------|-------------------------------------------------------------------------------------------------------------------|
| week01_foundation.html                          | activity-header                 | n/a               | ✅        | ✅       | Fixed      | week01/index.html                                                                                                 |
| Week01_lab1_dev_environment.html                | .step-header (event delegation) | ✅                | ✅        | ✅       | Fixed      | week01/lab1_dev_environment.html                                                                                  |
| week02_Core_Cloud_Services.html                 | tab layout (showTab)            | ✅                | n/a       | ✅       | Fixed      | week02/index.html                                                                                                 |
| week02_lab1_static_menu.html                    | .step-header (event delegation) | ✅                | ✅        | ✅       | Fixed      | week02/lab1_static_menu.html                                                                                      |
| week02_lab2_docker_networking.html              | .step-header (event delegation) | ✅                | ✅        | ✅       | Fixed      | week02/lab2_docker_networking.html                                                                                |
| week03_Databases_in_the_Cloud.html              | tab layout (showTab)            | ✅                | n/a       | ✅       | Fixed      | week03/index.html                                                                                                 |
| week03_lab1_docker_compose_mysql.html           | .step-header (parentElement)    | ✅                | ✅        | ✅       | Fixed      | week03/lab1_docker_compose_mysql.html                                                                             |
| week03_lab2_user_registration.html              | .step-header (parentElement)    | ✅                | ✅        | ✅       | Fixed      | week03/lab2_user_registration.html                                                                                |
| week04_Cloud_Native_Applications.html           | tab layout (showTab)            | ✅                | n/a       | ✅       | Fixed      | week04/index.html                                                                                                 |
| week04_lab1_relational_db_queries.html          | .step-header (event delegation) | ✅                | ✅        | ✅       | Fixed      | week04/lab1_relational_db_queries.html                                                                            |
| week04_lab2_nosql_orders.html                   | .step-header (event delegation) | ✅                | ✅        | ✅       | Fixed      | week04/lab2_nosql_orders.html                                                                                     |
| week05_Microservices_Architecture.html          | tab layout (showTab)            | ✅                | n/a       | ✅       | Fixed      | week05/index.html                                                                                                 |
| week05_lab1_microservices.html                  | .step-hd (ID-string)            | ✅                | ✅        | ✅       | Fixed ⚠️   | week05/lab1_microservices.html — beginner stop-here banner added after Part 4; Part 3 callout corrected (Phase 2 #5) |
| week05_lab2_api_gateway.html                    | .step-hd (ID-string)            | ✅                | ✅        | ✅       | Fixed      | week05/lab2_api_gateway.html                                                                                      |
| week06_DevOps_and_Version_Control.html          | tab layout (showTab)            | ✅                | n/a       | ✅       | Fixed      | week06/index.html                                                                                                 |
| week06_lab1_git_version_control.html            | .step-hd (ID-string)            | ✅                | ✅        | ✅       | Fixed      | week06/lab1_git_version_control.html                                                                              |
| week06_lab2_automated_testing.html              | .step-hd (ID-string)            | ✅                | ✅        | ✅       | Fixed ⚠️   | week06/lab2_automated_testing.html — CI/CD boundary callout added after Part 4 (Phase 2 #3)                       |
| week07_CICD_and_Infrastructure_as_Code.html     | tab layout (showTab)            | ✅                | n/a       | ✅       | Fixed      | week07/index.html                                                                                                 |
| week07_lab1_infrastructure_as_code.html         | .step-hd (ID-string)            | ✅                | ✅        | ✅       | Fixed      | week07/lab1_infrastructure_as_code.html                                                                           |
| week07_lab2_deployment_automation.html          | .step-hd (ID-string)            | ✅                | ✅        | ✅       | Fixed ⚠️   | week07/lab2_deployment_automation.html — CD boundary callout added before Part 1 (Phase 2 #3)                     |
| week08_Cloud_Security_and_Access_Control.html   | tab layout (showTab)            | ✅                | n/a       | ✅       | Fixed      | week08/index.html                                                                                                 |
| week08_lab1_jwt_authentication.html             | .step-header (toggleStep)       | ✅                | ✅        | ✅       | Fixed      | week08/lab1_jwt_authentication.html                                                                               |
| week08_lab2_rbac_access_control.html            | .step-header (toggleStep)       | ✅                | ✅        | ✅       | Fixed      | week08/lab2_rbac_access_control.html                                                                              |
| week09_Monitoring_Logging_and_Optimization.html | tab layout (showTab)            | ✅                | n/a       | ✅       | Fixed      | week09/index.html                                                                                                 |
| week09_lab1_application_logging.html            | .step-header (toggleStep)       | ✅                | ✅        | ✅       | Fixed      | week09/lab1_application_logging.html                                                                              |
| week09_lab2_performance_monitoring.html         | .step-header (toggleStep)       | ✅                | ✅        | ✅       | Fixed      | week09/lab2_performance_monitoring.html                                                                           |
| week10_Emerging_Trends_and_Course_Wrap.html     | tab layout (showTab)            | n/a               | n/a       | ✅       | Fixed      | week10/index.html — no code blocks; copyCode not applicable |
| week10_lab1_cloud_migration_plan.html           | .step-header (toggleStep)       | n/a               | ✅        | ✅       | Fixed      | week10/lab1_cloud_migration_plan.html — planning & worksheet lab only; all 15 `<code>` tags are inline component names, not runnable commands. No copy buttons needed. |

---

## Item #8 — CSS Extraction: Deferred

**Decision: defer to first maintenance cycle (post-launch).**

**Reason:** Content revision pass is still pending. Extracting shared CSS before content is finalised means any new CSS rule introduced during revision must be added to both the HTML file and the shared CSS file — double the touch points, higher error risk. Nothing is in Git yet, so there is no rollback if a scripted extraction breaks styles across all 29 files.

**Planned architecture when ready:**
- `assets/css/shared.css` — `:root` tokens, reset, body, typography, site-header, pace switcher, Google Fonts `@import`. Loaded by all 29 files.
- `assets/css/lecture.css` — tab layout, section headers, activity cards, hero. Loaded by 10 lecture files only.
- `assets/css/lab.css` — step/accordion, code blocks, callouts, checkpoints, pace-blocks, sidebar. Loaded by 18 lab files only.
- Each HTML file retains a minimal inline `<style>` for per-file token overrides only: `--lab-color`, `--week-color`, `--code-bg`.

**Trigger for execution:** after content revision pass is complete and all files are confirmed stable.
