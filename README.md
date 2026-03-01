# PhantomShield
A real-time Multi-Tier Supply Chain Finance (SCF) fraud detection engine. Uses Triple-Lock verification (Invoice-PO-GRN) and network topology mapping to identify phantom invoices and duplicate financing risks.

# Project Overview
PhantomShield is an automated risk management framework designed to protect lenders from multi-tier supply chain fraud. While traditional systems miss high-velocity "phantom" patterns PhantomShield unifies disparate data sources into a single verification layer.

# The Problem We Solve
Phantom Invoices: Detection of fabricated Tier 1 invoices  that lack physical delivery backing.

Cascading Exposure: Identifying risks that multiply as they move from Tier 3 to Tier 1.

Siloed Invisibility: Breaking data silos between lenders, buyers, and suppliers to reveal network-level correlation.

# Technical Pillars
The Triple-Lock System: Mandatory 3-way matching between Invoices, Purchase Orders (PO), and Goods Received Notes (GRN).

Invoice Fingerprinting: Generating unique digital signatures for every invoice to prevent "double dipping" (submitting the same invoice to multiple lenders).

Network Topology Mapping: Visualizing the buyer-supplier ecosystem to flag "orphan" nodes and sequencing anomalies.

Feasibility Scoring: Automated alerts when invoiced amounts exceed the supplier’s known logistical or production capacity.

# Final Implementation Plan 

Phase 1 (Data): Ingestion of multi-tier documentation (Invoices, POs, GRNs) into a unified relational schema.

Phase 2 (Logic): Deployment of the Triple-Lock Engine for real-time validation and Invoice Fingerprinting for duplicate detection.

Phase 3 (Analysis): Application of feasibility metrics and network topology mapping to identify phantom suppliers.

Phase 4 (Output): A pre-disbursement early warning dashboard for lenders to block fraudulent transactions in near real-time.
