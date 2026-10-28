\# CCSDS 902.13-M-1 & CSS-SM Abstract Event Definition (AED) Specification

\#\# Executive Summary  
This document provides the technical specification and architecture for \*\*AEDForge Pro\*\*, an industrial aerospace workstation implementing the \*\*Consultative Committee for Space Data Systems (CCSDS) 902.13-M-1\*\* Recommended Practice (\*Cross Support Service Management—Abstract Event Definition\*, Magenta Book, Issue 1, February 2021 with Technical Corrigendum 1, February 2024\) and \*\*ISO Cross Support Service Management (CSS-SM)\*\*.

In cross-support space mission operations, ground tracking stations and flight dynamics teams require a common, normative abstraction for representing time-tagged operational events. The \*\*Abstract Event Definition (AED)\*\* defines the underlying schema classes (\`AbstractEvent\`, \`AbstractEventTime\`, \`AbstractParameter\`), time-code representations (CCSDS ASCII Time Code A, Time Code B, and RelativeEventTime), duration definitions, and polymorphic parameter typings utilized by SSF (902.1), CPIF (902.2), SPDF (902.4), and EVSQ (902.6).

\#\# 1\. CSS-SM Structural Role of Abstract Event Definition  
Foundational layer for:  
\- Service Catalog (SECA): CCSDS 902.7-M-1 \[\#488\]  
\- Service Agreement & Profiles: CCSDS 902.5-B-1 (SACP) \[\#486\]  
\- Communications Planning: CCSDS 902.2-B-1 (CPIF) \[\#482\]  
\- Service Utilization Request: CCSDS 902.9-B-1 (SMURF) \[\#485\]  
\- Simple Schedule Agreement: CCSDS 902.1-B-1 (SSF) \[\#481\]  
\- Service Package Provisioning: CCSDS 902.4-B-1 (SPDF) \[\#483\]  
\- Event Sequence Execution: CCSDS 902.6-B-1 (EVSQ) \[\#484\]  
\- Service Accounting: CCSDS 902.8-B-1 (SMAC) \[\#487\]

\#\# 2\. Abstract Event Class Model (TC 1 Corrigendum)  
\- AbstractEvent: identifier (xsd:ID), type, user, description, earliestOffset, latestOffset.  
\- AbstractEventTime Polymorphism: CcsdsAsciiTimeCodeA (Calendar UTC), CcsdsAsciiTimeCodeB (Day of Year), RelativeEventTime (relative offset with otherEventRef).  
\- AbstractParameter: BooleanParameter, IntParameter, DoubleParameter, StringParameter, DurationDblParameter.  
