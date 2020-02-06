# Demo 2: Troubleshooting Guides & Status Page

>**Do you need to show videos instead of doing the demo live?:** Below, you'll find "stage-ready" videos that may be used in the event this presentation should be delivered offline.

|  | Video | Description
|--------|-------|-----|
| [Part 1: Troubleshooting Guide](#part-1-azure-troubleshooting-guide) | [Link](https://globaleventcdn.blob.core.windows.net/assets/ops/ops20/video/demo_2_full.mp4) | Deploy the Troubleshooting Guide via [Gallery template found here](TroubleshootingGuide_Gallery_Template.json) and discuss features
| [Part 2: Update Status Page](#part-2-update-status-page-from-microsoft-teams) | [Link](https://globaleventcdn.blob.core.windows.net/assets/ops/ops20/video/demo_2_full.mp4) | Demonstrate opening, updating, and closing a status announcement

---

**Question:** *What are we trying to demonstrate?*

**Answer :**
In this demonstration we want to highlight how Troubleshooting Guides can be customized in a way that they can be very useful in the early phases of response and remediation.

Additionally, we want to highlight the importance of sharing what information we have with a broader stakeholder audience. We should make clear and transparent communication of information a priority.

> **Presenter Setup Checklist:**

- [ ] [Troubleshooting Guide Gallery  template open in repo in a tab](TroubleshootingGuideGalleryTemplate.json)
- [ ] Status page is open in tab.
- [ ] Microsoft Teams open in browser tab (or native).
- [ ] Postman is open and ready to send the alert.

> Be sure all above are complete before beginning demo

## Part 1: Azure Troubleshooting Guide

We are going to use this as an opportunity to demonstrate how to create a new Troubleshooting guide using a template.

The troubleshooting guide web gallery template file (JSON) is found in this repository.

- [Gallery](TroubleshootingGuideGalleryTemplate.json)

We are using the gallery method as it seems to be more responsive for on-stage demos and much of the rest of the deployment is done using Gallery templates.

Once the Troubleshooting Guide has been created, begin exploring it.

>**Presenter Note:** If you haven't done so already, you will want to [follow the instructions to "Break the Tailwind Traders site"](../../deployment/break_tailwindtraders/README.md). Much of the functionality of the Troubleshooting Guide requires data from our monitoring services in order to populate anything interesting to demonstrate. You will want to break the deployment as soon as possible once you have verified everything else is ready to go.

## Part 2: Update Status Page from Microsoft Teams

To set the status of our Status Page to open, run the following from the chat field in Microsoft Teams:

``` Teams
@StatusPage open [message]
@StatusPage update [message]
@StatusPage close [message]
@StatusPage help [message]
```

![](https://globaleventcdn.blob.core.windows.net/assets/ops/ops20/screenshots/StatusPage.png)

>**Presenter Notes:** [More on the Microsoft Teams outgoing webhook can be found here](../../deployment/statuspage/README.md)
