---
title: Profiles defined as part of this Guide
layout: default
active: profiles
---

<!-- { :.no_toc } -->

<!-- TOC  the css styling for this is \pages\assets\css\project.css under 'markdown-toc'-->

* Do not remove this line (it will not be displayed)
{:toc}

<!-- end TOC -->

---
<br />

### Profiles

<table>
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="StructureDefinition-CCDA-on-FHIR-Care-Plan.html">C-CDA on FHIR Care Plan</a></td>
<td>CARE PLAN FRAMEWORK: A Care Plan (including Home Health Plan of Care (HHPoC)) is a consensus-driven dynamic plan that represents a patient and Care Team Members prioritized concerns, goals, and planned interventions. It serves as a blueprint shared by all Care Team Members (including the patient, their caregivers and providers), to guide the patients care. A Care Plan integrates multiple interventions proposed by multiple providers and disciplines for multiple conditions.

A Care Plan represents one or more Plan(s) of Care and serves to reconcile and resolve conflicts between the various Plans of Care developed for a specific patient by different providers. While both a plan of care and a care plan include the patient's life goals and require Care Team Members (including patients) to prioritize goals and interventions, the reconciliation process becomes more complex as the number of plans of care increases. The Care Plan also serves to enable longitudinal coordination of care.

The Care Plan represents an instance of this dynamic Care Plan at a point in time. The composition itself is NOT dynamic.

Key differentiators between a Care Plan profile and CCD  profile (another snapshot in time document):

*  Requires relationships between various concepts:

        *  Health Concerns

        *  Interventions

        *  Goals

        *  Outcomes

*  Provides the ability to identify patient and provider priorities with each act

*  Provides a header participant to indicate occurrences of Care Plan review</td>
</tr>
<tr>
<td><a href="StructureDefinition-CCDA-on-FHIR-Consent.html">C-CDA on FHIR Consent</a></td>
<td>This profile represents information about the patients consent.

The type of consent is conveyed in type. Consents in the header have been finalized and should be on file. This specification does not address how 'Privacy Consent' is represented, but does not preclude the inclusion of Privacy Consent.

The authorization consent is used for referring to consents that are documented elsewhere in the EHR or medical record for a health condition and/or treatment that is described in the document. </td>
</tr>
<tr>
<td><a href="StructureDefinition-CCDA-on-FHIR-Consultation-Note.html">C-CDA on FHIR Consultation Note</a></td>
<td>The Consultation Note is generated by a request from a clinician for an opinion or advice from another clinician. Consultations may involve face-to-face time with the patient or may fall under the auspices of telemedicine visits. Consultations may occur while the patient is inpatient or ambulatory. The Consultation Note should also be used to summarize an Emergency Room or Urgent Care encounter.

A Consultation Note includes the reason for the referral, history of present illness, physical examination, and decision-making components (Assessment and Plan). </td>
</tr>
<tr>
<td><a href="StructureDefinition-CCDA-on-FHIR-Continuity-of-Care-Document.html">C-CDA on FHIR Continuity of Care Document</a></td>
<td>This profile was originally based on the Continuity of Care Document (CCD) Release 1.1 which itself was derived from HITSP C32 and CCD Release 1.0.

The Continuity of Care Document (CCD) profile represents a core data set of the most relevant administrative, demographic, and clinical information facts about a patient's healthcare, covering one or more healthcare encounters. It provides a means for one healthcare practitioner, system, or setting to aggregate all of the pertinent data about a patient and forward it to another to support the continuity of care.  

The primary use case for the CCD is to provide a snapshot in time containing the germane clinical, demographic, and administrative data for a specific patient. The key characteristic of a CCD is that the Composition.event.code is constrained to "PCPR". This means it does not function to report new services associated with performing care. It reports on care that has already been provided. The CCD provides a historical tally of the care over a range of time and is not a record of new services delivered.

More specific use cases, such as a Discharge Summary, Transfer Summary, Referral Note, Consultation Note, or Progress Note, are available as alternative profiles. </td>
</tr>
<tr>
<td><a href="StructureDefinition-CCDA-on-FHIR-Diagnostic-Imaging-Report.html">C-CDA on FHIR Diagnostic Imaging Report</a></td>
<td>A Diagnostic Imaging Report (DIR) is a document that contains a consulting specialist's interpretation of image data. It conveys the interpretation to the referring (ordering) physician and becomes part of the patient's medical record. It is for use in Radiology, Endoscopy, Cardiology, and other imaging specialties. Note: this document type overlaps with the FHIR DiagnosticReport resource. Most use cases will want to use the specific resource type, but this document type is still useful for CDA to FHIR conversion and other such use cases. </td>
</tr>
<tr>
<td><a href="StructureDefinition-CCDA-on-FHIR-Discharge-Summary.html">C-CDA on FHIR Discharge Summary</a></td>
<td>The Discharge Summary is a document which synopsizes a patient's admission to a hospital, LTPAC provider, or other setting. It provides information for the continuation of care following discharge. The Joint Commission requires the following information to be included in the Discharge Summary (http://www.jointcommission.org/):

  The reason for hospitalization (the admission) 

  The procedures performed, as applicable

  The care, treatment, and services provided

  The patients condition and disposition at discharge

  Information provided to the patient and family

  Provisions for follow-up care

The best practice for a Discharge Summary is to include the discharge disposition in the display of the header.</td>
</tr>
<tr>
<td><a href="StructureDefinition-CCDA-on-FHIR-History-and-Physical.html">C-CDA on FHIR History and Physical</a></td>
<td>A History and Physical (H&P) note is a medical report that documents the current and past conditions of the patient. It contains essential information that helps determine an individual's health status.  

The first portion of the report is a current collection of organized information unique to an individual. This is typically supplied by the patient or the caregiver, concerning the current medical problem or the reason for the patient encounter. This information is followed by a description of any past or ongoing medical issues, including current medications and allergies. Information is also obtained about the patient's lifestyle, habits, and diseases among family members.
The next portion of the report contains information obtained by physically examining the patient and gathering diagnostic information in the form of laboratory tests, imaging, or other diagnostic procedures.
 
The report ends with the clinician's assessment of the patient's situation and the intended plan to address those issues.
 
A History and Physical Examination is required upon hospital admission as well as before operative procedures. An initial evaluation in an ambulatory setting is often documented in the form of an H&P note.</td>
</tr>
<tr>
<td><a href="StructureDefinition-CCDA-on-FHIR-Operative-Note.html">C-CDA on FHIR Operative Note</a></td>
<td>The Operative Note is a frequently used type of procedure note with specific requirements set forth by regulatory agencies.

The Operative Note is created immediately following a surgical or other high-risk procedure. It records the pre- and post-surgical diagnosis, pertinent events of the procedure, as well as the condition of the patient following the procedure. The report should be sufficiently detailed to support the diagnoses, justify the treatment, document the course of the procedure, and provide continuity of care. </td>
</tr>
<tr>
<td><a href="StructureDefinition-CCDA-on-FHIR-Procedure-Note.html">C-CDA on FHIR Procedure Note</a></td>
<td>A Procedure Note encompasses many types of non-operative procedures including interventional cardiology, gastrointestinal endoscopy, osteopathic manipulation, and many other specialty fields. Procedure Notes are differentiated from Operative Notes because they do not involve incision or excision as the primary act.

The Procedure Note is created immediately following a non-operative procedure. It records the indications for the procedure and, when applicable, postprocedure diagnosis, pertinent events of the procedure, and the patients tolerance for the procedure. It should be detailed enough to justify the procedure, describe the course of the procedure, and provide continuity of care. </td>
</tr>
<tr>
<td><a href="StructureDefinition-CCDA-on-FHIR-Progress-Note.html">C-CDA on FHIR Progress Note</a></td>
<td>This profile represents a patient's clinical status during a hospitalization, outpatient visit, treatment with a LTPAC provider, or other healthcare encounter.

Taber's medical dictionary defines a Progress Note as An ongoing record of a patient's illness and treatment. Physicians, nurses, consultants, and therapists record their notes concerning the progress or lack of progress made by the patient between the time of the previous note and the most recent note.

Mosby's medical dictionary defines a Progress Note as Notes made by a nurse, physician, social worker, physical therapist, and other health care professionals that describe the patient's condition and the treatment given or planned.

A Progress Note is not a re-evaluation note. A Progress Note is not intended to be a Progress Report for Medicare. Medicare B Section 1833(e) defines the requirements of a Medicare Progress Report. </td>
</tr>
<tr>
<td><a href="StructureDefinition-CCDA-on-FHIR-Referral-Note.html">C-CDA on FHIR Referral Note</a></td>
<td>A Referral Note communicates pertinent information from a provider who is requesting services of another provider of clinical or non-clinical services. The information in this document includes the reason for the referral and additional information that would augment decision making and care delivery.
 
Examples of referral situations are: 
* When a patient is referred from a family physician to a cardiologist for cardiac evaluation.
* When patient is sent by a cardiologist to an emergency department for angina.
* When a patient is referred by a nurse practitioner to an audiologist for hearing screening.
* When a patient is referred by a hospitalist to social services.</td>
</tr>
<tr>
<td><a href="StructureDefinition-CCDA-on-FHIR-Transfer-Summary.html">C-CDA on FHIR Transfer Summary</a></td>
<td>This profile describes constraints for a Transfer Summary. The Transfer Summary standardizes critical information for exchange of information between providers of care when a patient moves between health care settings. Standardization of information used in this form will promote interoperability; create information suitable for reuse in quality measurement, public health, research, and for reimbursement.</td>
</tr>
<tr>
<td><a href="StructureDefinition-CCDA-on-FHIR-US-Realm-Header.html">C-CDA on FHIR US Realm Header</a></td>
<td>This profile defines constraints that represent common administrative and demographic concepts for US Realm clinical documents. Further specification, such as type, are provided in document profiles that conform to this profile. </td>
</tr>
</tbody>
</table>


### Extensions

<table>
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="StructureDefinition-CCDA-on-FHIR-Authorization.html">C-CDA on FHIR Authorization</a></td>
<td>The C-CDA on FHIR Authorization Extension contains the C-CDA on FHIR Consent profile which represents information about a patient's consent.

For further information see the C-CDA specification here: http://www.hl7.org/implement/standards/product_brief.cfm?product_id=408.</td>
</tr>
<tr>
<td><a href="StructureDefinition-CCDA-on-FHIR-Data-Enterer.html">C-CDA on FHIR Data Enterer</a></td>
<td>The C-CDA on FHIR Data Enterer Extension represents the person who transferred the content, written or dictated, into the clinical document. To clarify, an author provides the content, subject to their own interpretation; a dataEnterer adds an author's information to the electronic system.

For further information see the C-CDA specification here: http://www.hl7.org/implement/standards/product_brief.cfm?product_id=408.</td>
</tr>
<tr>
<td><a href="StructureDefinition-CCDA-on-FHIR-In-Fulfillment-Of-Order.html">C-CDA on FHIR In Fulfillment Of Order</a></td>
<td>The C-CDA on FHIR In Fulfillment Of Order Extension represents orders that are fulfilled by this document such as a radiologists report of an x-ray.

For further information see the C-CDA specification here: http://www.hl7.org/implement/standards/product_brief.cfm?product_id=408.</td>
</tr>
<tr>
<td><a href="StructureDefinition-CCDA-on-FHIR-Informant.html">C-CDA on FHIR Informant</a></td>
<td>The C-CDA on FHIR Informant Extension describes an information source for any content within the clinical document. This informant is constrained for use when the source of information is an assigned health care provider for the patient.

For further information see the C-CDA specification here: http://www.hl7.org/implement/standards/product_brief.cfm?product_id=408.</td>
</tr>
<tr>
<td><a href="StructureDefinition-CCDA-on-FHIR-Information-Recipient.html">C-CDA on FHIR Information Recipient</a></td>
<td>The C-CDA on FHIR Information Recipient Extension records the intended recipient of the information at the time the document was created.

For further information see the C-CDA specification here: http://www.hl7.org/implement/standards/product_brief.cfm?product_id=408.</td>
</tr>
<tr>
<td><a href="StructureDefinition-CCDA-on-FHIR-Participant.html">C-CDA on FHIR Participant</a></td>
<td>The C-CDA on FHIR Participant Extension identifies supporting entities, including parents, relatives, caregivers, insurance policyholders, guarantors, and others related in some way to the patient. A supporting person or organization is an individual or an organization with a relationship to the patient. A supporting person who is playing multiple roles would be recorded in multiple participants (e.g., emergency contact and next-of-kin).

For further information see the C-CDA specification here: http://www.hl7.org/implement/standards/product_brief.cfm?product_id=408.</td>
</tr>
<tr>
<td><a href="StructureDefinition-CCDA-on-FHIR-Performer.html">C-CDA on FHIR Performer</a></td>
<td>The C-CDA on FHIR Performer Extension represents clinicians who actually and principally carry out the clinical services being documented. In a transfer of care this represents the healthcare providers involved in the current or pertinent historical care of the patient. Preferably, the patients key healthcare care team members would be listed, particularly their primary physician and any active consulting physicians, therapists, and counselors.

For further information see the C-CDA specification here: http://www.hl7.org/implement/standards/product_brief.cfm?product_id=408.</td>
</tr>
<tr>
<td><a href="StructureDefinition-CCDA-on-FHIR-VersionNumber.html">CCDA-on-FHIR-VersionNumber</a></td>
<td>The CCDA on FHIR VersionNumber Extension represents a numeric value used to version successive replacement documents.

For further information see the C-CDA specification here: http://www.hl7.org/implement/standards/product_brief.cfm?product_id=408.</td>
</tr>
</tbody>
</table>


