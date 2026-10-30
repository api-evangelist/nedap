# Nedap

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Nedap N.V. is a Dutch technology company founded in 1929 and listed on Euronext Amsterdam, headquartered in Groenlo, the Netherlands, with roughly 1,000 employees. It builds what it calls Digital Twin Technology across four markets — Healthcare (the Ons electronic health record suite and MediKIT for general practitioners), Livestock (cow monitoring), Retail (the iD Cloud RFID inventory platform and iSenseOS loss prevention) and Security (Nedap Access physical identity management and long-range vehicle/driver identification readers). Its most openly documented API surface is Ons API at ons-api.nl, a 926-operation OpenAPI 3.0.3 REST contract for the Ons care platform covering client dossiers, care planning, scheduling, rostering, payroll and finance, together with a 31-path openEHR composition and archetype surface, a webhook event service described in OpenAPI 3.1 webhooks, and a small scopes-and-clearances authorization API. A FHIR read/search surface built on the Dutch ZIB information models is documented but is not in the public specification — those endpoints sit behind the Ons API Dashboard. Access is gated on a client TLS certificate signed by Nedap's own CA and issued through the Ons API Dashboard, so the specifications are public while the runtime is not.

**Areas:** Company · Healthcare · Electronic Health Records · Interoperability · FHIR · openEHR · RFID · Retail · Physical Security · Livestock · Netherlands · Webhook

## Nedap on APIs.io

Everything profiled for Nedap is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/nedap/](https://apis.io/providers/nedap/)** — or go straight to one of the APIs or properties below.

### APIs (269)

- [Nedap Retail iD Cloud API](https://apis.io/apis/nedap/nedap-retail-id-cloud-api/) — The API for iD Cloud, Nedap's RFID item-level inventory platform for unified commerce, used to integrate store and supply-chain stock data with ERP and…
- [Nedap Address API](https://apis.io/apis/nedap/nedap-address-api/) — The Address API from Nedap — 15 operation(s) for address.
- [Nedap Admin.Background Image API](https://apis.io/apis/nedap/nedap-admin-backgroundimage-api/) — The admin.BackgroundImage API from Nedap — 2 operation(s) for admin.backgroundimage.
- [Nedap Admin.License API](https://apis.io/apis/nedap/nedap-admin-license-api/) — The admin.License API from Nedap — 2 operation(s) for admin.license.
- [Nedap Admin.Logo Image API](https://apis.io/apis/nedap/nedap-admin-logoimage-api/) — The admin.LogoImage API from Nedap — 4 operation(s) for admin.logoimage.
- [Nedap Admin.Timesheet Config API](https://apis.io/apis/nedap/nedap-admin-timesheetconfig-api/) — The admin.TimesheetConfig API from Nedap — 2 operation(s) for admin.timesheetconfig.
- [Nedap Admin.Version API](https://apis.io/apis/nedap/nedap-admin-version-api/) — The admin.Version API from Nedap — 2 operation(s) for admin.version.
- [Nedap Agbcode API](https://apis.io/apis/nedap/nedap-agbcode-api/) — The Agbcode API from Nedap — 6 operation(s) for agbcode.
- [Nedap Agenda.Agenda Occurrence API](https://apis.io/apis/nedap/nedap-agenda-agendaoccurrence-api/) — The agenda.AgendaOccurrence API from Nedap — 18 operation(s) for agenda.agendaoccurrence.
- [Nedap Agenda.Agenda Series API](https://apis.io/apis/nedap/nedap-agenda-agendaseries-api/) — The agenda.AgendaSeries API from Nedap — 6 operation(s) for agenda.agendaseries.
- [Nedap Agenda.Client Absence Occurrence API](https://apis.io/apis/nedap/nedap-agenda-clientabsenceoccurrence-api/) — The agenda.ClientAbsenceOccurrence API from Nedap — 4 operation(s) for agenda.clientabsenceoccurrence.
- [Nedap Agenda.Label API](https://apis.io/apis/nedap/nedap-agenda-label-api/) — The agenda.Label API from Nedap — 2 operation(s) for agenda.label.
- [Nedap Agenda.Registration Status API](https://apis.io/apis/nedap/nedap-agenda-registrationstatus-api/) — The agenda.RegistrationStatus API from Nedap — 2 operation(s) for agenda.registrationstatus.
- [Nedap Agenda.Reservation Create API](https://apis.io/apis/nedap/nedap-agenda-reservationcreate-api/) — The agenda.ReservationCreate API from Nedap — 2 operation(s) for agenda.reservationcreate.
- [Nedap Agenda.Reservation Occurrence API](https://apis.io/apis/nedap/nedap-agenda-reservationoccurrence-api/) — The agenda.ReservationOccurrence API from Nedap — 6 operation(s) for agenda.reservationoccurrence.
- [Nedap Agenda.Unavailability API](https://apis.io/apis/nedap/nedap-agenda-unavailability-api/) — The agenda.Unavailability API from Nedap — 2 operation(s) for agenda.unavailability.
- [Nedap Arrangement.Intent API](https://apis.io/apis/nedap/nedap-arrangement-intent-api/) — The arrangement.Intent API from Nedap — 10 operation(s) for arrangement.intent.
- [Nedap Arrangement.Intent Preference API](https://apis.io/apis/nedap/nedap-arrangement-intentpreference-api/) — The arrangement.IntentPreference API from Nedap — 10 operation(s) for arrangement.intentpreference.
- [Nedap Arrangement.Stakeholder API](https://apis.io/apis/nedap/nedap-arrangement-stakeholder-api/) — The arrangement.Stakeholder API from Nedap — 8 operation(s) for arrangement.stakeholder.
- [Nedap Arrangement.Time Slot API](https://apis.io/apis/nedap/nedap-arrangement-timeslot-api/) — The arrangement.TimeSlot API from Nedap — 10 operation(s) for arrangement.timeslot.
- [Nedap Authorization.provisioning.Default Scope API](https://apis.io/apis/nedap/nedap-authorization-provisioning-defaultscope-api/) — The authorization.provisioning.DefaultScope API from Nedap — 2 operation(s) for authorization.provisioning.defaultscope.
- [Nedap Authorization.provisioning.My Locations API](https://apis.io/apis/nedap/nedap-authorization-provisioning-mylocations-api/) — The authorization.provisioning.MyLocations API from Nedap — 2 operation(s) for authorization.provisioning.mylocations.
- [Nedap Authorization.provisioning.My Teams API](https://apis.io/apis/nedap/nedap-authorization-provisioning-myteams-api/) — The authorization.provisioning.MyTeams API from Nedap — 2 operation(s) for authorization.provisioning.myteams.
- [Nedap Authorization.provisioning.Role API](https://apis.io/apis/nedap/nedap-authorization-provisioning-role-api/) — The authorization.provisioning.Role API from Nedap — 2 operation(s) for authorization.provisioning.role.
- [Nedap Authorization.provisioning.User API](https://apis.io/apis/nedap/nedap-authorization-provisioning-user-api/) — The authorization.provisioning.User API from Nedap — 2 operation(s) for authorization.provisioning.user.
- [Nedap Authorization.provisioning.User Duties API](https://apis.io/apis/nedap/nedap-authorization-provisioning-userduties-api/) — The authorization.provisioning.UserDuties API from Nedap — 2 operation(s) for authorization.provisioning.userduties.
- [Nedap Authorization.provisioning.User Scope Settings API](https://apis.io/apis/nedap/nedap-authorization-provisioning-userscopesettings-api/) — The authorization.provisioning.UserScopeSettings API from Nedap — 2 operation(s) for authorization.provisioning.userscopesettings.
- [Nedap Bsn API](https://apis.io/apis/nedap/nedap-bsn-api/) — The Bsn API from Nedap — 6 operation(s) for bsn.
- [Nedap Capacity.Capacity Profile API](https://apis.io/apis/nedap/nedap-capacity-capacityprofile-api/) — The capacity.CapacityProfile API from Nedap — 6 operation(s) for capacity.capacityprofile.
- [Nedap Care Allocation API](https://apis.io/apis/nedap/nedap-careallocation-api/) — The CareAllocation API from Nedap — 12 operation(s) for careallocation.
- [Nedap Care Arrangement API](https://apis.io/apis/nedap/nedap-carearrangement-api/) — The CareArrangement API from Nedap — 6 operation(s) for carearrangement.
- [Nedap Carepath.Care Path API](https://apis.io/apis/nedap/nedap-carepath-carepath-api/) — The carepath.CarePath API from Nedap — 4 operation(s) for carepath.carepath.
- [Nedap Carepath.Template API](https://apis.io/apis/nedap/nedap-carepath-template-api/) — The carepath.Template API from Nedap — 4 operation(s) for carepath.template.
- [Nedap Care Provider API](https://apis.io/apis/nedap/nedap-careprovider-api/) — The CareProvider API from Nedap — 16 operation(s) for careprovider.
- [Nedap Care Provider Address API](https://apis.io/apis/nedap/nedap-careprovideraddress-api/) — The CareProviderAddress API from Nedap — 4 operation(s) for careprovideraddress.
- [Nedap Caretech.Order API](https://apis.io/apis/nedap/nedap-caretech-order-api/) — The caretech.Order API from Nedap — 6 operation(s) for caretech.order.
- [Nedap Caretech.Product Allocation API](https://apis.io/apis/nedap/nedap-caretech-productallocation-api/) — The caretech.ProductAllocation API from Nedap — 2 operation(s) for caretech.productallocation.
- [Nedap Caretech.Return Request API](https://apis.io/apis/nedap/nedap-caretech-returnrequest-api/) — The caretech.ReturnRequest API from Nedap — 6 operation(s) for caretech.returnrequest.
- [Nedap Client API](https://apis.io/apis/nedap/nedap-client-api/) — The Client API from Nedap — 42 operation(s) for client.
- [Nedap Client Story.Change Set API](https://apis.io/apis/nedap/nedap-client-story-changeset-api/) — The client_story.ChangeSet API from Nedap — 2 operation(s) for client_story.changeset.
- [Nedap Client Story.Story API](https://apis.io/apis/nedap/nedap-client-story-story-api/) — The client_story.Story API from Nedap — 14 operation(s) for client_story.story.
- [Nedap Client Absence API](https://apis.io/apis/nedap/nedap-clientabsence-api/) — The ClientAbsence API from Nedap — 10 operation(s) for clientabsence.
- [Nedap Client Absence Reason API](https://apis.io/apis/nedap/nedap-clientabsencereason-api/) — The ClientAbsenceReason API from Nedap — 4 operation(s) for clientabsencereason.
- [Nedap Client Address API](https://apis.io/apis/nedap/nedap-clientaddress-api/) — The ClientAddress API from Nedap — 8 operation(s) for clientaddress.
- [Nedap Client Card API](https://apis.io/apis/nedap/nedap-clientcard-api/) — The ClientCard API from Nedap — 2 operation(s) for clientcard.
- [Nedap Client Contact Relation API](https://apis.io/apis/nedap/nedap-clientcontactrelation-api/) — The ClientContactRelation API from Nedap — 12 operation(s) for clientcontactrelation.
- [Nedap Client Contact Relation Address API](https://apis.io/apis/nedap/nedap-clientcontactrelationaddress-api/) — The ClientContactRelationAddress API from Nedap — 8 operation(s) for clientcontactrelationaddress.
- [Nedap Client Contact Relation Type API](https://apis.io/apis/nedap/nedap-clientcontactrelationtype-api/) — The ClientContactRelationType API from Nedap — 4 operation(s) for clientcontactrelationtype.
- [Nedap Client Employee Relation API](https://apis.io/apis/nedap/nedap-clientemployeerelation-api/) — The ClientEmployeeRelation API from Nedap — 8 operation(s) for clientemployeerelation.
- [Nedap Client Employee Relation Type API](https://apis.io/apis/nedap/nedap-clientemployeerelationtype-api/) — The ClientEmployeeRelationType API from Nedap — 4 operation(s) for clientemployeerelationtype.
- [Nedap Clients In Care API](https://apis.io/apis/nedap/nedap-clientsincare-api/) — The ClientsInCare API from Nedap — 4 operation(s) for clientsincare.
- [Nedap Cost Center Selection Option API](https://apis.io/apis/nedap/nedap-costcenterselectionoption-api/) — The CostCenterSelectionOption API from Nedap — 2 operation(s) for costcenterselectionoption.
- [Nedap Dashboard Profile API](https://apis.io/apis/nedap/nedap-dashboardprofile-api/) — The DashboardProfile API from Nedap — 2 operation(s) for dashboardprofile.
- [Nedap Dbc.DBC Sub Traject API](https://apis.io/apis/nedap/nedap-dbc-dbcsubtraject-api/) — The dbc.DBCSubTraject API from Nedap — 6 operation(s) for dbc.dbcsubtraject.
- [Nedap Dbc.DBC Traject API](https://apis.io/apis/nedap/nedap-dbc-dbctraject-api/) — The dbc.DBCTraject API from Nedap — 4 operation(s) for dbc.dbctraject.
- [Nedap Dbc.ggz.Diagnose Toekenning API](https://apis.io/apis/nedap/nedap-dbc-ggz-diagnosetoekenning-api/) — The dbc.ggz.DiagnoseToekenning API from Nedap — 2 operation(s) for dbc.ggz.diagnosetoekenning.
- [Nedap Dbc.ggz.fz.Subtraject API](https://apis.io/apis/nedap/nedap-dbc-ggz-fz-subtraject-api/) — The dbc.ggz.fz.Subtraject API from Nedap — 6 operation(s) for dbc.ggz.fz.subtraject.
- [Nedap Dbc.ggz.Presence Log Synchronisation Error API](https://apis.io/apis/nedap/nedap-dbc-ggz-presencelogsynchronisationerror-api/) — The dbc.ggz.PresenceLogSynchronisationError API from Nedap — 4 operation(s) for dbc.ggz.presencelogsynchronisationerror.
- [Nedap Dbc.ggz.Subtraject API](https://apis.io/apis/nedap/nedap-dbc-ggz-subtraject-api/) — The dbc.ggz.Subtraject API from Nedap — 10 operation(s) for dbc.ggz.subtraject.
- [Nedap Dbc.ggz.Validation Error API](https://apis.io/apis/nedap/nedap-dbc-ggz-validationerror-api/) — The dbc.ggz.ValidationError API from Nedap — 4 operation(s) for dbc.ggz.validationerror.
- [Nedap Dbc.ggz.Zorgtraject API](https://apis.io/apis/nedap/nedap-dbc-ggz-zorgtraject-api/) — The dbc.ggz.Zorgtraject API from Nedap — 6 operation(s) for dbc.ggz.zorgtraject.
- [Nedap Debtor API](https://apis.io/apis/nedap/nedap-debtor-api/) — The Debtor API from Nedap — 10 operation(s) for debtor.
- [Nedap Dienst Verwijzen Module.Bundle Wrapper API](https://apis.io/apis/nedap/nedap-dienst-verwijzen-module-bundlewrapper-api/) — The dienst_verwijzen_module.BundleWrapper API from Nedap — 2 operation(s) for dienst_verwijzen_module.bundlewrapper.
- [Nedap Document API](https://apis.io/apis/nedap/nedap-document-api/) — The Document API from Nedap — 17 operation(s) for document.
- [Nedap Dossier.Action API](https://apis.io/apis/nedap/nedap-dossier-action-api/) — The dossier.Action API from Nedap — 12 operation(s) for dossier.action.
- [Nedap Dossier.Action Entry API](https://apis.io/apis/nedap/nedap-dossier-actionentry-api/) — The dossier.ActionEntry API from Nedap — 6 operation(s) for dossier.actionentry.
- [Nedap Dossier.Action Entry Summary API](https://apis.io/apis/nedap/nedap-dossier-actionentrysummary-api/) — The dossier.ActionEntrySummary API from Nedap — 2 operation(s) for dossier.actionentrysummary.
- [Nedap Dossier.Active Care Plan Metadata API](https://apis.io/apis/nedap/nedap-dossier-activecareplanmetadata-api/) — The dossier.ActiveCarePlanMetadata API from Nedap — 2 operation(s) for dossier.activecareplanmetadata.
- [Nedap Dossier.admin.alerts.Topic API](https://apis.io/apis/nedap/nedap-dossier-admin-alerts-topic-api/) — The dossier.admin.alerts.Topic API from Nedap — 4 operation(s) for dossier.admin.alerts.topic.
- [Nedap Dossier.Alert API](https://apis.io/apis/nedap/nedap-dossier-alert-api/) — The dossier.Alert API from Nedap — 8 operation(s) for dossier.alert.
- [Nedap Dossier.Care Plan API](https://apis.io/apis/nedap/nedap-dossier-careplan-api/) — The dossier.CarePlan API from Nedap — 16 operation(s) for dossier.careplan.
- [Nedap Dossier.Care Plan Agreement API](https://apis.io/apis/nedap/nedap-dossier-careplanagreement-api/) — The dossier.CarePlanAgreement API from Nedap — 2 operation(s) for dossier.careplanagreement.
- [Nedap Dossier.Care Plan Entry API](https://apis.io/apis/nedap/nedap-dossier-careplanentry-api/) — The dossier.CarePlanEntry API from Nedap — 8 operation(s) for dossier.careplanentry.
- [Nedap Dossier.Care Plan Report Right API](https://apis.io/apis/nedap/nedap-dossier-careplanreportright-api/) — The dossier.CarePlanReportRight API from Nedap — 2 operation(s) for dossier.careplanreportright.
- [Nedap Dossier.Care Plan Signature Requirement API](https://apis.io/apis/nedap/nedap-dossier-careplansignaturerequirement-api/) — The dossier.CarePlanSignatureRequirement API from Nedap — 2 operation(s) for dossier.careplansignaturerequirement.
- [Nedap Dossier.Client Note API](https://apis.io/apis/nedap/nedap-dossier-clientnote-api/) — The dossier.ClientNote API from Nedap — 6 operation(s) for dossier.clientnote.
- [Nedap Dossier.Demand API](https://apis.io/apis/nedap/nedap-dossier-demand-api/) — The dossier.Demand API from Nedap — 8 operation(s) for dossier.demand.
- [Nedap Dossier.Demand Entry API](https://apis.io/apis/nedap/nedap-dossier-demandentry-api/) — The dossier.DemandEntry API from Nedap — 4 operation(s) for dossier.demandentry.
- [Nedap Dossier.Domain API](https://apis.io/apis/nedap/nedap-dossier-domain-api/) — The dossier.Domain API from Nedap — 6 operation(s) for dossier.domain.
- [Nedap Dossier.episodes.Action API](https://apis.io/apis/nedap/nedap-dossier-episodes-action-api/) — The dossier.episodes.Action API from Nedap — 8 operation(s) for dossier.episodes.action.
- [Nedap Dossier.episodes.Episode API](https://apis.io/apis/nedap/nedap-dossier-episodes-episode-api/) — The dossier.episodes.Episode API from Nedap — 6 operation(s) for dossier.episodes.episode.
- [Nedap Dossier.episodes.Sub Goal API](https://apis.io/apis/nedap/nedap-dossier-episodes-subgoal-api/) — The dossier.episodes.SubGoal API from Nedap — 6 operation(s) for dossier.episodes.subgoal.
- [Nedap Dossier.Goal API](https://apis.io/apis/nedap/nedap-dossier-goal-api/) — The dossier.Goal API from Nedap — 12 operation(s) for dossier.goal.
- [Nedap Dossier.Goal Entry API](https://apis.io/apis/nedap/nedap-dossier-goalentry-api/) — The dossier.GoalEntry API from Nedap — 4 operation(s) for dossier.goalentry.
- [Nedap Dossier.Involuntary Care Export Entry API](https://apis.io/apis/nedap/nedap-dossier-involuntarycareexportentry-api/) — The dossier.InvoluntaryCareExportEntry API from Nedap — 2 operation(s) for dossier.involuntarycareexportentry.
- [Nedap Dossier.Last Medical Moment API](https://apis.io/apis/nedap/nedap-dossier-lastmedicalmoment-api/) — The dossier.LastMedicalMoment API from Nedap — 2 operation(s) for dossier.lastmedicalmoment.
- [Nedap Dossier.medical.advance Directives.Context API](https://apis.io/apis/nedap/nedap-dossier-medical-advance-directives-context-api/) — The dossier.medical.advance_directives.Context API from Nedap — 6 operation(s) for dossier.medical.advance_directives.context.
- [Nedap Dossier.medical.dsm.Classification API](https://apis.io/apis/nedap/nedap-dossier-medical-dsm-classification-api/) — The dossier.medical.dsm.Classification API from Nedap — 4 operation(s) for dossier.medical.dsm.classification.
- [Nedap Dossier.medical.dsm.Classification Series API](https://apis.io/apis/nedap/nedap-dossier-medical-dsm-classificationseries-api/) — The dossier.medical.dsm.ClassificationSeries API from Nedap — 7 operation(s) for dossier.medical.dsm.classificationseries.
- [Nedap Dossier.medical.involuntary Care.Incompetence API](https://apis.io/apis/nedap/nedap-dossier-medical-involuntary-care-incompetence-api/) — The dossier.medical.involuntary_care.Incompetence API from Nedap — 4 operation(s) for dossier.medical.involuntary_care.incompetence.
- [Nedap Dossier.medical.involuntary Care.Legal Status API](https://apis.io/apis/nedap/nedap-dossier-medical-involuntary-care-legalstatus-api/) — The dossier.medical.involuntary_care.LegalStatus API from Nedap — 6 operation(s) for dossier.medical.involuntary_care.legalstatus.
- [Nedap Dossier.medical.Medical Summary API](https://apis.io/apis/nedap/nedap-dossier-medical-medicalsummary-api/) — The dossier.medical.MedicalSummary API from Nedap — 2 operation(s) for dossier.medical.medicalsummary.
- [Nedap Dossier.medical.Problem API](https://apis.io/apis/nedap/nedap-dossier-medical-problem-api/) — The dossier.medical.Problem API from Nedap — 4 operation(s) for dossier.medical.problem.
- [Nedap Dossier.medical.Propensity To Adverse Reaction API](https://apis.io/apis/nedap/nedap-dossier-medical-propensitytoadversereaction-api/) — The dossier.medical.PropensityToAdverseReaction API from Nedap — 6 operation(s) for dossier.medical.propensitytoadversereaction.
- [Nedap Dossier.medical.Simplified Propensity To Adverse Reaction API](https://apis.io/apis/nedap/nedap-dossier-medical-simplifiedpropensitytoadversereaction-api/) — The dossier.medical.SimplifiedPropensityToAdverseReaction API from Nedap — 2 operation(s) for dossier.medical.simplifiedpropensitytoadversereaction.
- [Nedap Dossier.Medical Note API](https://apis.io/apis/nedap/nedap-dossier-medicalnote-api/) — The dossier.MedicalNote API from Nedap — 8 operation(s) for dossier.medicalnote.
- [Nedap Dossier.omaha.Classified Problem API](https://apis.io/apis/nedap/nedap-dossier-omaha-classifiedproblem-api/) — The dossier.omaha.ClassifiedProblem API from Nedap — 4 operation(s) for dossier.omaha.classifiedproblem.
- [Nedap Dossier.omaha.Intervention Category API](https://apis.io/apis/nedap/nedap-dossier-omaha-interventioncategory-api/) — The dossier.omaha.InterventionCategory API from Nedap — 2 operation(s) for dossier.omaha.interventioncategory.
- [Nedap Dossier.omaha.Intervention Target API](https://apis.io/apis/nedap/nedap-dossier-omaha-interventiontarget-api/) — The dossier.omaha.InterventionTarget API from Nedap — 2 operation(s) for dossier.omaha.interventiontarget.
- [Nedap Dossier.omaha.Omaha Classification API](https://apis.io/apis/nedap/nedap-dossier-omaha-omahaclassification-api/) — The dossier.omaha.OmahaClassification API from Nedap — 6 operation(s) for dossier.omaha.omahaclassification.
- [Nedap Dossier.omaha.Problem API](https://apis.io/apis/nedap/nedap-dossier-omaha-problem-api/) — The dossier.omaha.Problem API from Nedap — 2 operation(s) for dossier.omaha.problem.
- [Nedap Dossier.Report API](https://apis.io/apis/nedap/nedap-dossier-report-api/) — The dossier.Report API from Nedap — 52 operation(s) for dossier.report.
- [Nedap Dossier.Report Type API](https://apis.io/apis/nedap/nedap-dossier-reporttype-api/) — The dossier.ReportType API from Nedap — 4 operation(s) for dossier.reporttype.
- [Nedap Dossier.Report With Actions API](https://apis.io/apis/nedap/nedap-dossier-reportwithactions-api/) — The dossier.ReportWithActions API from Nedap — 2 operation(s) for dossier.reportwithactions.
- [Nedap Dossier.Restrictive Measure Care Plan Entry API](https://apis.io/apis/nedap/nedap-dossier-restrictivemeasurecareplanentry-api/) — The dossier.RestrictiveMeasureCarePlanEntry API from Nedap — 6 operation(s) for dossier.restrictivemeasurecareplanentry.
- [Nedap Dossier.Restrictive Measure Registration API](https://apis.io/apis/nedap/nedap-dossier-restrictivemeasureregistration-api/) — The dossier.RestrictiveMeasureRegistration API from Nedap — 6 operation(s) for dossier.restrictivemeasureregistration.
- [Nedap Dossier.System Note API](https://apis.io/apis/nedap/nedap-dossier-systemnote-api/) — The dossier.SystemNote API from Nedap — 4 operation(s) for dossier.systemnote.
- [Nedap Employee API](https://apis.io/apis/nedap/nedap-employee-api/) — The Employee API from Nedap — 28 operation(s) for employee.
- [Nedap Employee Address API](https://apis.io/apis/nedap/nedap-employeeaddress-api/) — The EmployeeAddress API from Nedap — 8 operation(s) for employeeaddress.
- [Nedap Employee Privacy Settings API](https://apis.io/apis/nedap/nedap-employeeprivacysettings-api/) — The EmployeePrivacySettings API from Nedap — 2 operation(s) for employeeprivacysettings.
- [Nedap Employee Workflow API](https://apis.io/apis/nedap/nedap-employeeworkflow-api/) — The EmployeeWorkflow API from Nedap — 4 operation(s) for employeeworkflow.
- [Nedap Evs.Evs Ability API](https://apis.io/apis/nedap/nedap-evs-evsability-api/) — The evs.EvsAbility API from Nedap — 2 operation(s) for evs.evsability.
- [Nedap Evs.Response Message API](https://apis.io/apis/nedap/nedap-evs-responsemessage-api/) — The evs.ResponseMessage API from Nedap — 2 operation(s) for evs.responsemessage.
- [Nedap Expense.Expense API](https://apis.io/apis/nedap/nedap-expense-expense-api/) — The expense.Expense API from Nedap — 10 operation(s) for expense.expense.
- [Nedap Expense.Expense Address Model API](https://apis.io/apis/nedap/nedap-expense-expenseaddressmodel-api/) — The expense.ExpenseAddressModel API from Nedap — 4 operation(s) for expense.expenseaddressmodel.
- [Nedap Expense.Expense Type API](https://apis.io/apis/nedap/nedap-expense-expensetype-api/) — The expense.ExpenseType API from Nedap — 4 operation(s) for expense.expensetype.
- [Nedap Expertise Group API](https://apis.io/apis/nedap/nedap-expertisegroup-api/) — The ExpertiseGroup API from Nedap — 10 operation(s) for expertisegroup.
- [Nedap Expertise Profile API](https://apis.io/apis/nedap/nedap-expertiseprofile-api/) — The ExpertiseProfile API from Nedap — 12 operation(s) for expertiseprofile.
- [Nedap Expertise Profile Assignment API](https://apis.io/apis/nedap/nedap-expertiseprofileassignment-api/) — The ExpertiseProfileAssignment API from Nedap — 14 operation(s) for expertiseprofileassignment.
- [Nedap Export.Export Presence Log API](https://apis.io/apis/nedap/nedap-export-exportpresencelog-api/) — The export.ExportPresenceLog API from Nedap — 6 operation(s) for export.exportpresencelog.
- [Nedap Finance.Care Order API](https://apis.io/apis/nedap/nedap-finance-careorder-api/) — The finance.CareOrder API from Nedap — 14 operation(s) for finance.careorder.
- [Nedap Finance.Care Order Product API](https://apis.io/apis/nedap/nedap-finance-careorderproduct-api/) — The finance.CareOrderProduct API from Nedap — 10 operation(s) for finance.careorderproduct.
- [Nedap Finance.Client Financed Product API](https://apis.io/apis/nedap/nedap-finance-clientfinancedproduct-api/) — The finance.ClientFinancedProduct API from Nedap — 4 operation(s) for finance.clientfinancedproduct.
- [Nedap Finance.Debtor Group API](https://apis.io/apis/nedap/nedap-finance-debtorgroup-api/) — The finance.DebtorGroup API from Nedap — 6 operation(s) for finance.debtorgroup.
- [Nedap Finance.Declaration Rule API](https://apis.io/apis/nedap/nedap-finance-declarationrule-api/) — The finance.DeclarationRule API from Nedap — 10 operation(s) for finance.declarationrule.
- [Nedap Finance.Export Profile API](https://apis.io/apis/nedap/nedap-finance-exportprofile-api/) — The finance.ExportProfile API from Nedap — 4 operation(s) for finance.exportprofile.
- [Nedap Finance.Finance Log API](https://apis.io/apis/nedap/nedap-finance-financelog-api/) — The finance.FinanceLog API from Nedap — 4 operation(s) for finance.financelog.
- [Nedap Finance.Finance Type API](https://apis.io/apis/nedap/nedap-finance-financetype-api/) — The finance.FinanceType API from Nedap — 6 operation(s) for finance.financetype.
- [Nedap Finance.Forensic Care Order API](https://apis.io/apis/nedap/nedap-finance-forensiccareorder-api/) — The finance.ForensicCareOrder API from Nedap — 4 operation(s) for finance.forensiccareorder.
- [Nedap Finance.Group Activity Suggestion Model API](https://apis.io/apis/nedap/nedap-finance-groupactivitysuggestionmodel-api/) — The finance.GroupActivitySuggestionModel API from Nedap — 4 operation(s) for finance.groupactivitysuggestionmodel.
- [Nedap Finance.Invoice API](https://apis.io/apis/nedap/nedap-finance-invoice-api/) — The finance.Invoice API from Nedap — 4 operation(s) for finance.invoice.
- [Nedap Finance.Invoice Provider Group API](https://apis.io/apis/nedap/nedap-finance-invoiceprovidergroup-api/) — The finance.InvoiceProviderGroup API from Nedap — 2 operation(s) for finance.invoiceprovidergroup.
- [Nedap Finance.Invoice Row API](https://apis.io/apis/nedap/nedap-finance-invoicerow-api/) — The finance.InvoiceRow API from Nedap — 4 operation(s) for finance.invoicerow.
- [Nedap Finance.Invoice Row Finance Log API](https://apis.io/apis/nedap/nedap-finance-invoicerowfinancelog-api/) — The finance.InvoiceRowFinanceLog API from Nedap — 2 operation(s) for finance.invoicerowfinancelog.
- [Nedap Finance.Parallel Care Order API](https://apis.io/apis/nedap/nedap-finance-parallelcareorder-api/) — The finance.ParallelCareOrder API from Nedap — 2 operation(s) for finance.parallelcareorder.
- [Nedap Finance.Product API](https://apis.io/apis/nedap/nedap-finance-product-api/) — The finance.Product API from Nedap — 8 operation(s) for finance.product.
- [Nedap Finance.Restitution API](https://apis.io/apis/nedap/nedap-finance-restitution-api/) — The finance.Restitution API from Nedap — 4 operation(s) for finance.restitution.
- [Nedap Finance.Vecozo Invoice Relation API](https://apis.io/apis/nedap/nedap-finance-vecozoinvoicerelation-api/) — The finance.VecozoInvoiceRelation API from Nedap — 4 operation(s) for finance.vecozoinvoicerelation.
- [Nedap Free Field Assignment API](https://apis.io/apis/nedap/nedap-freefieldassignment-api/) — The FreeFieldAssignment API from Nedap — 4 operation(s) for freefieldassignment.
- [Nedap Free Field Category API](https://apis.io/apis/nedap/nedap-freefieldcategory-api/) — The FreeFieldCategory API from Nedap — 2 operation(s) for freefieldcategory.
- [Nedap Free Field Definition API](https://apis.io/apis/nedap/nedap-freefielddefinition-api/) — The FreeFieldDefinition API from Nedap — 2 operation(s) for freefielddefinition.
- [Nedap Fvc.Fvc Message API](https://apis.io/apis/nedap/nedap-fvc-fvcmessage-api/) — The fvc.FvcMessage API from Nedap — 2 operation(s) for fvc.fvcmessage.
- [Nedap Groepsplanning.Group API](https://apis.io/apis/nedap/nedap-groepsplanning-group-api/) — The groepsplanning.Group API from Nedap — 2 operation(s) for groepsplanning.group.
- [Nedap Groupcare.Group API](https://apis.io/apis/nedap/nedap-groupcare-group-api/) — The groupcare.Group API from Nedap — 6 operation(s) for groupcare.group.
- [Nedap Groupcare.Occurrence API](https://apis.io/apis/nedap/nedap-groupcare-occurrence-api/) — The groupcare.Occurrence API from Nedap — 2 operation(s) for groupcare.occurrence.
- [Nedap Harmony.Zorgdomein Fhir Connector API](https://apis.io/apis/nedap/nedap-harmony-zorgdomeinfhirconnector-api/) — The harmony.ZorgdomeinFhirConnector API from Nedap — 2 operation(s) for harmony.zorgdomeinfhirconnector.
- [Nedap Herald.Announcement Count API](https://apis.io/apis/nedap/nedap-herald-announcementcount-api/) — The herald.AnnouncementCount API from Nedap — 2 operation(s) for herald.announcementcount.
- [Nedap Hermes.Care Provider Settings API](https://apis.io/apis/nedap/nedap-hermes-careprovidersettings-api/) — The hermes.CareProviderSettings API from Nedap — 2 operation(s) for hermes.careprovidersettings.
- [Nedap Hermes.Contact Method API](https://apis.io/apis/nedap/nedap-hermes-contactmethod-api/) — The hermes.ContactMethod API from Nedap — 4 operation(s) for hermes.contactmethod.
- [Nedap Hermes.Notification API](https://apis.io/apis/nedap/nedap-hermes-notification-api/) — The hermes.Notification API from Nedap — 8 operation(s) for hermes.notification.
- [Nedap Hour Type Category API](https://apis.io/apis/nedap/nedap-hourtypecategory-api/) — The HourTypeCategory API from Nedap — 6 operation(s) for hourtypecategory.
- [Nedap Hour Type Product Assignment API](https://apis.io/apis/nedap/nedap-hourtypeproductassignment-api/) — The HourTypeProductAssignment API from Nedap — 6 operation(s) for hourtypeproductassignment.
- [Nedap Insurance API](https://apis.io/apis/nedap/nedap-insurance-api/) — The Insurance API from Nedap — 10 operation(s) for insurance.
- [Nedap Jw.Jw Zorglegitimatie API](https://apis.io/apis/nedap/nedap-jw-jwzorglegitimatie-api/) — The jw.JwZorglegitimatie API from Nedap — 4 operation(s) for jw.jwzorglegitimatie.
- [Nedap Kamino.Kamino Setting API](https://apis.io/apis/nedap/nedap-kamino-kaminosetting-api/) — The kamino.KaminoSetting API from Nedap — 2 operation(s) for kamino.kaminosetting.
- [Nedap Location API](https://apis.io/apis/nedap/nedap-location-api/) — The Location API from Nedap — 14 operation(s) for location.
- [Nedap Location Assignment API](https://apis.io/apis/nedap/nedap-locationassignment-api/) — The LocationAssignment API from Nedap — 12 operation(s) for locationassignment.
- [Nedap Location Assignment Residence API](https://apis.io/apis/nedap/nedap-locationassignmentresidence-api/) — The LocationAssignmentResidence API from Nedap — 6 operation(s) for locationassignmentresidence.
- [Nedap Location Assignment Waiting List API](https://apis.io/apis/nedap/nedap-locationassignmentwaitinglist-api/) — The LocationAssignmentWaitingList API from Nedap — 6 operation(s) for locationassignmentwaitinglist.
- [Nedap Medication.Double Check API](https://apis.io/apis/nedap/nedap-medication-doublecheck-api/) — The medication.DoubleCheck API from Nedap — 2 operation(s) for medication.doublecheck.
- [Nedap Medication.Double Check Change API](https://apis.io/apis/nedap/nedap-medication-doublecheckchange-api/) — The medication.DoubleCheckChange API from Nedap — 2 operation(s) for medication.doublecheckchange.
- [Nedap Medication.Medication Administration API](https://apis.io/apis/nedap/nedap-medication-medicationadministration-api/) — The medication.MedicationAdministration API from Nedap — 4 operation(s) for medication.medicationadministration.
- [Nedap Medication.Medication Plan API](https://apis.io/apis/nedap/nedap-medication-medicationplan-api/) — The medication.MedicationPlan API from Nedap — 6 operation(s) for medication.medicationplan.
- [Nedap Milo.Device API](https://apis.io/apis/nedap/nedap-milo-device-api/) — The milo.Device API from Nedap — 12 operation(s) for milo.device.
- [Nedap Moves.Absence API](https://apis.io/apis/nedap/nedap-moves-absence-api/) — The moves.Absence API from Nedap — 4 operation(s) for moves.absence.
- [Nedap Moves.Availability API](https://apis.io/apis/nedap/nedap-moves-availability-api/) — The moves.Availability API from Nedap — 6 operation(s) for moves.availability.
- [Nedap Moves.Availability Type API](https://apis.io/apis/nedap/nedap-moves-availabilitytype-api/) — The moves.AvailabilityType API from Nedap — 2 operation(s) for moves.availabilitytype.
- [Nedap Moves.Client Planned Schedule Planned Visit API](https://apis.io/apis/nedap/nedap-moves-clientplannedscheduleplannedvisit-api/) — The moves.ClientPlannedSchedulePlannedVisit API from Nedap — 2 operation(s) for moves.clientplannedscheduleplannedvisit.
- [Nedap Moves.Client Planning Filter API](https://apis.io/apis/nedap/nedap-moves-clientplanningfilter-api/) — The moves.ClientPlanningFilter API from Nedap — 2 operation(s) for moves.clientplanningfilter.
- [Nedap Moves.Container API](https://apis.io/apis/nedap/nedap-moves-container-api/) — The moves.Container API from Nedap — 2 operation(s) for moves.container.
- [Nedap Moves.Employee Export Job API](https://apis.io/apis/nedap/nedap-moves-employeeexportjob-api/) — The moves.EmployeeExportJob API from Nedap — 4 operation(s) for moves.employeeexportjob.
- [Nedap Moves.Employee Hours Report API](https://apis.io/apis/nedap/nedap-moves-employeehoursreport-api/) — The moves.EmployeeHoursReport API from Nedap — 2 operation(s) for moves.employeehoursreport.
- [Nedap Moves.Employee Moves Profile API](https://apis.io/apis/nedap/nedap-moves-employeemovesprofile-api/) — The moves.EmployeeMovesProfile API from Nedap — 2 operation(s) for moves.employeemovesprofile.
- [Nedap Moves.Employee Planning API](https://apis.io/apis/nedap/nedap-moves-employeeplanning-api/) — The moves.EmployeePlanning API from Nedap — 4 operation(s) for moves.employeeplanning.
- [Nedap Moves.Employee Schedule API](https://apis.io/apis/nedap/nedap-moves-employeeschedule-api/) — The moves.EmployeeSchedule API from Nedap — 2 operation(s) for moves.employeeschedule.
- [Nedap Moves.Expertise Profile API](https://apis.io/apis/nedap/nedap-moves-expertiseprofile-api/) — The moves.ExpertiseProfile API from Nedap — 6 operation(s) for moves.expertiseprofile.
- [Nedap Moves.Flex Signup API](https://apis.io/apis/nedap/nedap-moves-flexsignup-api/) — The moves.FlexSignup API from Nedap — 2 operation(s) for moves.flexsignup.
- [Nedap Moves.Membership API](https://apis.io/apis/nedap/nedap-moves-membership-api/) — The moves.Membership API from Nedap — 6 operation(s) for moves.membership.
- [Nedap Moves.Navigation Availability API](https://apis.io/apis/nedap/nedap-moves-navigationavailability-api/) — The moves.NavigationAvailability API from Nedap — 2 operation(s) for moves.navigationavailability.
- [Nedap Moves.Plan Card Occurrence API](https://apis.io/apis/nedap/nedap-moves-plancardoccurrence-api/) — The moves.PlanCardOccurrence API from Nedap — 6 operation(s) for moves.plancardoccurrence.
- [Nedap Moves.Planned Visit API](https://apis.io/apis/nedap/nedap-moves-plannedvisit-api/) — The moves.PlannedVisit API from Nedap — 4 operation(s) for moves.plannedvisit.
- [Nedap Moves.Roster Slot API](https://apis.io/apis/nedap/nedap-moves-rosterslot-api/) — The moves.RosterSlot API from Nedap — 14 operation(s) for moves.rosterslot.
- [Nedap Moves.Shift API](https://apis.io/apis/nedap/nedap-moves-shift-api/) — The moves.Shift API from Nedap — 8 operation(s) for moves.shift.
- [Nedap Moves.Shift Assignment API](https://apis.io/apis/nedap/nedap-moves-shiftassignment-api/) — The moves.ShiftAssignment API from Nedap — 4 operation(s) for moves.shiftassignment.
- [Nedap Moves.Team API](https://apis.io/apis/nedap/nedap-moves-team-api/) — The moves.Team API from Nedap — 6 operation(s) for moves.team.
- [Nedap Moves.Unit API](https://apis.io/apis/nedap/nedap-moves-unit-api/) — The moves.Unit API from Nedap — 6 operation(s) for moves.unit.
- [Nedap Moves.Working Employee Report API](https://apis.io/apis/nedap/nedap-moves-workingemployeereport-api/) — The moves.WorkingEmployeeReport API from Nedap — 2 operation(s) for moves.workingemployeereport.
- [Nedap Navigation Availability API](https://apis.io/apis/nedap/nedap-navigationavailability-api/) — The NavigationAvailability API from Nedap — 2 operation(s) for navigationavailability.
- [Nedap Nexus.Client Contact Relation Type API](https://apis.io/apis/nedap/nedap-nexus-clientcontactrelationtype-api/) — The nexus.ClientContactRelationType API from Nedap — 4 operation(s) for nexus.clientcontactrelationtype.
- [Nedap Nexus.Client Employee Relation API](https://apis.io/apis/nedap/nedap-nexus-clientemployeerelation-api/) — The nexus.ClientEmployeeRelation API from Nedap — 12 operation(s) for nexus.clientemployeerelation.
- [Nedap Nexus.Client Employee Relation Type API](https://apis.io/apis/nedap/nedap-nexus-clientemployeerelationtype-api/) — The nexus.ClientEmployeeRelationType API from Nedap — 4 operation(s) for nexus.clientemployeerelationtype.
- [Nedap Nexus.Organisation Category API](https://apis.io/apis/nedap/nedap-nexus-organisationcategory-api/) — The nexus.OrganisationCategory API from Nedap — 4 operation(s) for nexus.organisationcategory.
- [Nedap Nexus.Personal Relation Type API](https://apis.io/apis/nedap/nedap-nexus-personalrelationtype-api/) — The nexus.PersonalRelationType API from Nedap — 4 operation(s) for nexus.personalrelationtype.
- [Nedap Nuts.Consent API](https://apis.io/apis/nedap/nedap-nuts-consent-api/) — The nuts.Consent API from Nedap — 4 operation(s) for nuts.consent.
- [Nedap Ons Administration.Employee Workdays Overview Model API](https://apis.io/apis/nedap/nedap-ons-administration-employeeworkdaysoverviewmodel-api/) — The ons_administration.EmployeeWorkdaysOverviewModel API from Nedap — 2 operation(s) for ons_administration.employeeworkdaysoverviewmodel.
- [Nedap Ons Administration.Extended Employee Model API](https://apis.io/apis/nedap/nedap-ons-administration-extendedemployeemodel-api/) — The ons_administration.ExtendedEmployeeModel API from Nedap — 2 operation(s) for ons_administration.extendedemployeemodel.
- [Nedap Ons Administration.Time Compensation Factor Model API](https://apis.io/apis/nedap/nedap-ons-administration-timecompensationfactormodel-api/) — The ons_administration.TimeCompensationFactorModel API from Nedap — 2 operation(s) for ons_administration.timecompensationfactormodel.
- [Nedap Ons Administration.Workday Hour Type Model API](https://apis.io/apis/nedap/nedap-ons-administration-workdayhourtypemodel-api/) — The ons_administration.WorkdayHourTypeModel API from Nedap — 2 operation(s) for ons_administration.workdayhourtypemodel.
- [Nedap Ons Administration.Workday Norm Period Model API](https://apis.io/apis/nedap/nedap-ons-administration-workdaynormperiodmodel-api/) — The ons_administration.WorkdayNormPeriodModel API from Nedap — 2 operation(s) for ons_administration.workdaynormperiodmodel.
- [Nedap Ons Administration.Workday Norm Settings Model API](https://apis.io/apis/nedap/nedap-ons-administration-workdaynormsettingsmodel-api/) — The ons_administration.WorkdayNormSettingsModel API from Nedap — 8 operation(s) for ons_administration.workdaynormsettingsmodel.
- [Nedap Ons Client.Shared Resource API](https://apis.io/apis/nedap/nedap-ons-client-sharedresource-api/) — The ons_client.SharedResource API from Nedap — 2 operation(s) for ons_client.sharedresource.
- [Nedap Ons Ehr.Ggz Plan Statistics API](https://apis.io/apis/nedap/nedap-ons-ehr-ggzplanstatistics-api/) — The ons_ehr.GgzPlanStatistics API from Nedap — 2 operation(s) for ons_ehr.ggzplanstatistics.
- [Nedap Ons Ehr.Last Visited Plan API](https://apis.io/apis/nedap/nedap-ons-ehr-lastvisitedplan-api/) — The ons_ehr.LastVisitedPlan API from Nedap — 2 operation(s) for ons_ehr.lastvisitedplan.
- [Nedap Ons Ehr.Navigation Availability API](https://apis.io/apis/nedap/nedap-ons-ehr-navigationavailability-api/) — The ons_ehr.NavigationAvailability API from Nedap — 2 operation(s) for ons_ehr.navigationavailability.
- [Nedap Ons Ehr.Setting API](https://apis.io/apis/nedap/nedap-ons-ehr-setting-api/) — The ons_ehr.Setting API from Nedap — 2 operation(s) for ons_ehr.setting.
- [Nedap Ons API Clearance Response API](https://apis.io/apis/nedap/nedap-onsapiclearanceresponse-api/) — The OnsApiClearanceResponse API from Nedap — 2 operation(s) for onsapiclearanceresponse.
- [Nedap Ons API Scope Response API](https://apis.io/apis/nedap/nedap-onsapiscoperesponse-api/) — The OnsApiScopeResponse API from Nedap — 2 operation(s) for onsapiscoperesponse.
- [Nedap Onsimport.Run API](https://apis.io/apis/nedap/nedap-onsimport-run-api/) — The onsimport.Run API from Nedap — 22 operation(s) for onsimport.run.
- [Nedap Openehr.Archetype Wrapper API](https://apis.io/apis/nedap/nedap-openehr-archetypewrapper-api/) — The openehr.ArchetypeWrapper API from Nedap — 10 operation(s) for openehr.archetypewrapper.
- [Nedap Openehr.Care Plan Vvt Care Profile Link API](https://apis.io/apis/nedap/nedap-openehr-careplanvvtcareprofilelink-api/) — The openehr.CarePlanVvtCareProfileLink API from Nedap — 2 operation(s) for openehr.careplanvvtcareprofilelink.
- [Nedap Openehr.Composition Wrapper API](https://apis.io/apis/nedap/nedap-openehr-compositionwrapper-api/) — The openehr.CompositionWrapper API from Nedap — 23 operation(s) for openehr.compositionwrapper.
- [Nedap Openehr.Employee Group API](https://apis.io/apis/nedap/nedap-openehr-employeegroup-api/) — The openehr.EmployeeGroup API from Nedap — 6 operation(s) for openehr.employeegroup.
- [Nedap Openehr.Item Tag API](https://apis.io/apis/nedap/nedap-openehr-itemtag-api/) — The openehr.ItemTag API from Nedap — 4 operation(s) for openehr.itemtag.
- [Nedap Openehr.Multimedia File API](https://apis.io/apis/nedap/nedap-openehr-multimediafile-api/) — The openehr.MultimediaFile API from Nedap — 8 operation(s) for openehr.multimediafile.
- [Nedap Payroll.Account Entry API](https://apis.io/apis/nedap/nedap-payroll-accountentry-api/) — The payroll.AccountEntry API from Nedap — 14 operation(s) for payroll.accountentry.
- [Nedap Payroll.Account Type API](https://apis.io/apis/nedap/nedap-payroll-accounttype-api/) — The payroll.AccountType API from Nedap — 4 operation(s) for payroll.accounttype.
- [Nedap Payroll.Account Type Expire Statistic API](https://apis.io/apis/nedap/nedap-payroll-accounttypeexpirestatistic-api/) — The payroll.AccountTypeExpireStatistic API from Nedap — 2 operation(s) for payroll.accounttypeexpirestatistic.
- [Nedap Payroll.Collective Agreement API](https://apis.io/apis/nedap/nedap-payroll-collectiveagreement-api/) — The payroll.CollectiveAgreement API from Nedap — 4 operation(s) for payroll.collectiveagreement.
- [Nedap Payroll.Collective Agreement Assignment API](https://apis.io/apis/nedap/nedap-payroll-collectiveagreementassignment-api/) — The payroll.CollectiveAgreementAssignment API from Nedap — 6 operation(s) for payroll.collectiveagreementassignment.
- [Nedap Payroll.Collective Agreement Rule API](https://apis.io/apis/nedap/nedap-payroll-collectiveagreementrule-api/) — The payroll.CollectiveAgreementRule API from Nedap — 4 operation(s) for payroll.collectiveagreementrule.
- [Nedap Payroll.Contract API](https://apis.io/apis/nedap/nedap-payroll-contract-api/) — The payroll.Contract API from Nedap — 10 operation(s) for payroll.contract.
- [Nedap Payroll.Contract Type API](https://apis.io/apis/nedap/nedap-payroll-contracttype-api/) — The payroll.ContractType API from Nedap — 4 operation(s) for payroll.contracttype.
- [Nedap Payroll.holiday.Holiday API](https://apis.io/apis/nedap/nedap-payroll-holiday-holiday-api/) — The payroll.holiday.Holiday API from Nedap — 4 operation(s) for payroll.holiday.holiday.
- [Nedap Payroll.Hourly Wage API](https://apis.io/apis/nedap/nedap-payroll-hourlywage-api/) — The payroll.HourlyWage API from Nedap — 8 operation(s) for payroll.hourlywage.
- [Nedap Payroll.Payable Hours Average API](https://apis.io/apis/nedap/nedap-payroll-payablehoursaverage-api/) — The payroll.PayableHoursAverage API from Nedap — 8 operation(s) for payroll.payablehoursaverage.
- [Nedap Payroll.Work Hours Balance API](https://apis.io/apis/nedap/nedap-payroll-workhoursbalance-api/) — The payroll.WorkHoursBalance API from Nedap — 8 operation(s) for payroll.workhoursbalance.
- [Nedap Payroll.Work Load API](https://apis.io/apis/nedap/nedap-payroll-workload-api/) — The payroll.WorkLoad API from Nedap — 2 operation(s) for payroll.workload.
- [Nedap Personal Relation Type API](https://apis.io/apis/nedap/nedap-personalrelationtype-api/) — The PersonalRelationType API from Nedap — 4 operation(s) for personalrelationtype.
- [Nedap Portal.Employee Portal Profile API](https://apis.io/apis/nedap/nedap-portal-employeeportalprofile-api/) — The portal.EmployeePortalProfile API from Nedap — 2 operation(s) for portal.employeeportalprofile.
- [Nedap Practitioner API](https://apis.io/apis/nedap/nedap-practitioner-api/) — The Practitioner API from Nedap — 6 operation(s) for practitioner.
- [Nedap Practitioner Agb Code API](https://apis.io/apis/nedap/nedap-practitioneragbcode-api/) — The PractitionerAgbCode API from Nedap — 4 operation(s) for practitioneragbcode.
- [Nedap Practitioner Big Code API](https://apis.io/apis/nedap/nedap-practitionerbigcode-api/) — The PractitionerBigCode API from Nedap — 4 operation(s) for practitionerbigcode.
- [Nedap Practitioner Profession API](https://apis.io/apis/nedap/nedap-practitionerprofession-api/) — The PractitionerProfession API from Nedap — 4 operation(s) for practitionerprofession.
- [Nedap Presence Log API](https://apis.io/apis/nedap/nedap-presencelog-api/) — The PresenceLog API from Nedap — 13 operation(s) for presencelog.
- [Nedap Profile Activity Assignment API](https://apis.io/apis/nedap/nedap-profileactivityassignment-api/) — The ProfileActivityAssignment API from Nedap — 14 operation(s) for profileactivityassignment.
- [Nedap Referral API](https://apis.io/apis/nedap/nedap-referral-api/) — The Referral API from Nedap — 8 operation(s) for referral.
- [Nedap Skn API](https://apis.io/apis/nedap/nedap-skn-api/) — The Skn API from Nedap — 2 operation(s) for skn.
- [Nedap Status.Application Status API](https://apis.io/apis/nedap/nedap-status-applicationstatus-api/) — The status.ApplicationStatus API from Nedap — 2 operation(s) for status.applicationstatus.
- [Nedap Survey.Answer API](https://apis.io/apis/nedap/nedap-survey-answer-api/) — The survey.Answer API from Nedap — 2 operation(s) for survey.answer.
- [Nedap Survey.Answer Definition Group API](https://apis.io/apis/nedap/nedap-survey-answerdefinitiongroup-api/) — The survey.AnswerDefinitionGroup API from Nedap — 4 operation(s) for survey.answerdefinitiongroup.
- [Nedap Survey.Group Answer API](https://apis.io/apis/nedap/nedap-survey-groupanswer-api/) — The survey.GroupAnswer API from Nedap — 2 operation(s) for survey.groupanswer.
- [Nedap Survey.Survey API](https://apis.io/apis/nedap/nedap-survey-survey-api/) — The survey.Survey API from Nedap — 6 operation(s) for survey.survey.
- [Nedap Survey.Survey Result API](https://apis.io/apis/nedap/nedap-survey-surveyresult-api/) — The survey.SurveyResult API from Nedap — 10 operation(s) for survey.surveyresult.
- [Nedap Tasque.Care Task Group API](https://apis.io/apis/nedap/nedap-tasque-caretaskgroup-api/) — The tasque.CareTaskGroup API from Nedap — 4 operation(s) for tasque.caretaskgroup.
- [Nedap Tasque.Care Task Group Status API](https://apis.io/apis/nedap/nedap-tasque-caretaskgroupstatus-api/) — The tasque.CareTaskGroupStatus API from Nedap — 2 operation(s) for tasque.caretaskgroupstatus.
- [Nedap Tasque.Care Task Occurrence API](https://apis.io/apis/nedap/nedap-tasque-caretaskoccurrence-api/) — The tasque.CareTaskOccurrence API from Nedap — 38 operation(s) for tasque.caretaskoccurrence.
- [Nedap Tasque.Care Task Series API](https://apis.io/apis/nedap/nedap-tasque-caretaskseries-api/) — The tasque.CareTaskSeries API from Nedap — 2 operation(s) for tasque.caretaskseries.
- [Nedap Team API](https://apis.io/apis/nedap/nedap-team-api/) — The Team API from Nedap — 22 operation(s) for team.
- [Nedap Team Address API](https://apis.io/apis/nedap/nedap-teamaddress-api/) — The TeamAddress API from Nedap — 4 operation(s) for teamaddress.
- [Nedap Team Assignment API](https://apis.io/apis/nedap/nedap-teamassignment-api/) — The TeamAssignment API from Nedap — 12 operation(s) for teamassignment.
- [Nedap Toezicht.Audit API](https://apis.io/apis/nedap/nedap-toezicht-audit-api/) — The toezicht.Audit API from Nedap — 2 operation(s) for toezicht.audit.
- [Nedap Transport.Client Transport API](https://apis.io/apis/nedap/nedap-transport-clienttransport-api/) — The transport.ClientTransport API from Nedap — 2 operation(s) for transport.clienttransport.
- [Nedap Treatment Location API](https://apis.io/apis/nedap/nedap-treatmentlocation-api/) — The TreatmentLocation API from Nedap — 2 operation(s) for treatmentlocation.
- [Nedap User API](https://apis.io/apis/nedap/nedap-user-api/) — The User API from Nedap — 28 operation(s) for user.
- [Nedap Vehicle Assignment Model API](https://apis.io/apis/nedap/nedap-vehicleassignmentmodel-api/) — The VehicleAssignmentModel API from Nedap — 4 operation(s) for vehicleassignmentmodel.
- [Nedap Weeksheet Profile API](https://apis.io/apis/nedap/nedap-weeksheetprofile-api/) — The WeeksheetProfile API from Nedap — 6 operation(s) for weeksheetprofile.
- [Nedap Whismur.Care Provider Setting API](https://apis.io/apis/nedap/nedap-whismur-careprovidersetting-api/) — The whismur.CareProviderSetting API from Nedap — 2 operation(s) for whismur.careprovidersetting.
- [Nedap Wlz.Wlz Zorglegitimatie API](https://apis.io/apis/nedap/nedap-wlz-wlzzorglegitimatie-api/) — The wlz.WlzZorglegitimatie API from Nedap — 4 operation(s) for wlz.wlzzorglegitimatie.
- [Nedap Wmo.Wmo Zorglegitimatie API](https://apis.io/apis/nedap/nedap-wmo-wmozorglegitimatie-api/) — The wmo.WmoZorglegitimatie API from Nedap — 4 operation(s) for wmo.wmozorglegitimatie.
- [Nedap Worksheet.Worksheet API](https://apis.io/apis/nedap/nedap-worksheet-worksheet-api/) — The worksheet.Worksheet API from Nedap — 2 operation(s) for worksheet.worksheet.
- [Nedap Zorgdomein Module.Bundle Wrapper API](https://apis.io/apis/nedap/nedap-zorgdomein-module-bundlewrapper-api/) — The zorgdomein_module.BundleWrapper API from Nedap — 2 operation(s) for zorgdomein_module.bundlewrapper.
- [Nedap Zorgmail Module.Diagnostic Procedure API](https://apis.io/apis/nedap/nedap-zorgmail-module-diagnosticprocedure-api/) — The zorgmail_module.DiagnosticProcedure API from Nedap — 2 operation(s) for zorgmail_module.diagnosticprocedure.
- [Nedap Zorgmail Module.Zorgmail Mailbox Dto API](https://apis.io/apis/nedap/nedap-zorgmail-module-zorgmailmailboxdto-api/) — The zorgmail_module.ZorgmailMailboxDto API from Nedap — 2 operation(s) for zorgmail_module.zorgmailmailboxdto.
- [Nedap Zpm.Care Order Zpm Details API](https://apis.io/apis/nedap/nedap-zpm-careorderzpmdetails-api/) — The zpm.CareOrderZpmDetails API from Nedap — 4 operation(s) for zpm.careorderzpmdetails.
- [Nedap Zpm.Zpm Gbggz Profiel API](https://apis.io/apis/nedap/nedap-zpm-zpmgbggzprofiel-api/) — The zpm.ZpmGbggzProfiel API from Nedap — 2 operation(s) for zpm.zpmgbggzprofiel.
- [Nedap Zpm.Zpm Setting API](https://apis.io/apis/nedap/nedap-zpm-zpmsetting-api/) — The zpm.ZpmSetting API from Nedap — 2 operation(s) for zpm.zpmsetting.
- [Nedap Zpm.Zpm Zorglabel API](https://apis.io/apis/nedap/nedap-zpm-zpmzorglabel-api/) — The zpm.ZpmZorglabel API from Nedap — 2 operation(s) for zpm.zpmzorglabel.
- [Nedap Bank Account API](https://apis.io/apis/nedap/nedap-bank-account-api/) — The Bank Account API from Nedap — 6 operation(s) for bank account.
- [Nedap Hour Type API](https://apis.io/apis/nedap/nedap-hour-type-api/) — The Hour Type API from Nedap — 8 operation(s) for hour type.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Nedap Ons Webhooks](https://apis.io/asyncapis/nedap/nedap-ons-webhooks/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [nedap-mcp.yml](https://apis.io/servers/nedap/nedap-mcp-yml/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Nedap Ons Overlay](https://apis.io/overlays/nedap/nedap-ons-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Nedap Authentication](https://apis.io/security/nedap/nedap-authentication/)
- [Nedap Domain Security](https://apis.io/security/nedap/nedap-domain-security/)
- [Nedap Vulnerability Disclosure](https://apis.io/security/nedap/nedap-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Nedap Plans Pricing](https://apis.io/plans/nedap/nedap-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Nedap Rate Limits](https://apis.io/rate-limits/nedap/nedap-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.nedap.com/en)
- [Documentation](https://ons-api.nl/english/technical/technical.html)
- [Getting started](https://ons-api.nl/english/integration_process/Integration_process.html)
- [API reference](https://ons-api.nl/english/technical/APIS.html)
- [Sign up](https://api-dashboard.ons.io/intake)
- [Support](https://support.nedap-ons.nl/)
- [Blog](https://www.nedap.com/en/news)
- [Security](https://www.nedap.com/en/coordinated-vulnerability-disclosure-policy)
- [Terms of service](https://www.nedap.com/en/terms-and-conditions)
- [Privacy policy](https://www.nedap.com/en/privacy-statement-disclaimer)
- [GitHub](https://github.com/nedap)
- [Status](https://support.nedap-ons.nl/)

## API Evangelist rating

**Kin Score 61.7** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 78.6 |
| Contract quality | 51.8 |
| Contract governance | 18.2 |
| Operational transparency | 97.4 |
| Developer ergonomics | 73.2 |
| Access clarity | 21.1 |

**Agent readiness 29.8** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | partial |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | yes |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | — |

**Regulatory alignment 24.2** — Health

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/nedap/](https://apis.io/providers/nedap/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Nedap: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/nedap/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
