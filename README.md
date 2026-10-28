\# AEDForge Pro (v1.0.0)  
\*\*CCSDS 902.13-M-1 & CSS-SM Abstract Event Definition (AED) Workstation\*\*    
\*Aerospace Ground Station Cross-Support Abstract Event Modeling Studio, Event Graph & Time Code Transcoder, SANA Schema Auditor\*

\#\# Overview  
AEDForge Pro is an industrial-grade aerospace workstation implementing the CCSDS 902.13-M-1 Recommended Practice (Cross Support Service Management—Abstract Event Definition, Magenta Book, Issue 1, February 2021 with Technical Corrigendum 1, February 2024\) and ISO Cross Support Service Management (CSS-SM).

In cross-support space mission operations, ground tracking stations and flight dynamics teams require a common, normative abstraction for representing time-tagged operational events. The Abstract Event Definition (AED) establishes the foundational schema classes (AbstractEvent, AbstractEventTime, AbstractParameter), time-code formats (Time Code A, Time Code B, and RelativeEventTime), duration definitions, and polymorphic parameter typings utilized by SSF (902.1), CPIF (902.2), SPDF (902.4), and EVSQ (902.6).

AEDForge Pro delivers a zero-dependency ES6 engine, interactive Glass-Cockpit web console, multi-subcommand Python 3 CLI, and a 10-point normative aerospace compliance auditor ensuring automated AbstractEvent construction, bidirectional time-code transcoding, polymorphic parameter typing, event graph topological ordering, and SANA XML (902x13m01TC1-AED.xsd) and KVN export.

\#\# Key Capabilities  
1\. Normative AbstractEvent Modeling: Formalizes unique event identifiers (xsd:ID), event type strings, operating user references, descriptions, and execution jitter tolerance bounds (earliestOffset and latestOffset).  
2\. Bidirectional Time Code Transcoder: Converts seamlessly between CCSDS ASCII Time Code A (YYYY-MM-DDTHH:MM:SS.sssZ Calendar UTC) and CCSDS ASCII Time Code B (YYYY-DDDTHH:MM:SS.sssZ Day of Year) with leap year arithmetic.  
3\. Relative Event Timing & IDREF Traversal: Resolves relative delta offsets (relativeTime) anchored to parent event nodes via otherEventRef (xsd:IDREF).  
4\. Polymorphic Parameter Typing: Enforces strongly typed parameters matching SANA schema subclasses: BooleanParameter, IntParameter, DoubleParameter, StringParameter, and non-negative DurationDblParameter.  
5\. Topological DAG Event Graph Resolver: Sorts complex multi-event dependencies into monotonic chronological execution orders with zero circular loops.  
6\. 10-Point Normative Compliance Auditor: Automates validation against CCSDS 902.13-M-1 requirements (§3.2 through §5.3), achieving a 100% pass rate (CCSDS\_902\_13\_AED\_CERTIFIED).  
7\. Bilateral XML & KVN Serializer: Exports valid XML conforming to SANA CSS-SM schema 902x13m01TC1-AED.xsd (urn:ccsds:schema:csssm:aed) and clean Key-Value Notation (KVN).

\#\# Commercial Licensing & Enterprise Support  
\- Professional Seat: \$4,950 / year (Single flight operations engineer)  
\- Enterprise Site License: \$49,500 / year (Unlimited seats, custom telemetry driver plugins, MOC API integration support)  
\- Standards Conformance: CCSDS 902.13-M-1, CCSDS 301.0-B, CCSDS 902.12-M-1, ISO CSS-SM.  
