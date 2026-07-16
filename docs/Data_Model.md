## Project Entities
1. Person
2. Political Party
3. Position
4. Election
5. Institution
6. Event
7. Source
8. Media
   
## Relationships
Person attends Institution

Person belongs to Political Party

Person holds Position

Person contests Election

Person participates in Event


# Kenya Political Archive
## Data Model (Version 1.0)

---

# Purpose

This document defines the core entities, relationships, and design principles of the Kenya Political Archive database.

The goal is to create a scalable, normalized, and interconnected knowledge base capable of storing Kenyan political history from 1963 to the present.

---

# Design Principles

1. Every entity has a unique identifier (UUID).
2. Every fact must reference at least one source.
3. No duplicate information should exist.
4. Relationships should be stored separately from entities whenever possible.
5. Historical records should never be overwritten; changes should create new records where appropriate.
6. The system should support AI-powered search and knowledge graph queries.

---

# Core Entities

## 1. Person

Represents an individual.

Examples:

- Jomo Kenyatta
- Daniel arap Moi
- Raila Odinga
- William Ruto

A Person can have:

- Multiple schools
- Multiple political parties
- Multiple positions
- Multiple elections
- Multiple speeches
- Multiple achievements
- Multiple controversies
- Multiple photos

---

## 2. Political Party

Represents a registered political party.

Examples:

- KANU
- ODM
- Jubilee
- UDA

---

## 3. Position

Represents a political office.

Examples:

- President
- Vice President
- Deputy President
- Cabinet Minister
- Cabinet Secretary
- Member of Parliament
- Senator
- Governor

---

## 4. Institution

Represents an organization.

Examples:

- Alliance High School
- University of Nairobi
- Parliament of Kenya
- Kenya Army

Institution Types

- School
- University
- Government
- Military
- NGO
- Company
- Religious Organization

---

## 5. Election

Represents an election.

Examples:

- 1963 General Election
- 1992 General Election
- 2022 General Election

---

## 6. Event

Represents historical events.

Examples:

- Independence
- 1982 Coup Attempt
- 2007 Post-Election Violence
- 2010 Constitution Promulgation

---

## 7. Source

Represents where information came from.

Examples:

- Newspaper
- Book
- Court Judgment
- Hansard
- Kenya Gazette
- Official Biography

---

## 8. Media

Represents digital assets.

Examples:

- Photos
- Videos
- Audio
- PDFs
- Documents

---

# Relationships

A Person may:

- Attend an Institution
- Join a Political Party
- Hold a Position
- Contest an Election
- Participate in an Event
- Have a Relationship with another Person
- Own or Direct a Company
- Receive an Award
- Deliver a Speech
- Publish a Book
- Be connected to one or more Sources
- Have multiple Media files

---

# Relationship Examples

William Ruto

↓

Attended

↓

Kapsabet High School

----------------------------

William Ruto

↓

Belongs To

↓

United Democratic Alliance

----------------------------

William Ruto

↓

Held Position

↓

Deputy President

2013–2022

----------------------------

William Ruto

↓

Contested

↓

2022 Presidential Election

----------------------------

William Ruto

↓

Related To

↓

Rigathi Gachagua

Political Ally (Historical)

---

# Source Requirement

Every factual statement must reference one or more Source records.

No source = No fact.

---

# Future Expansion

Future entities may include:

- County
- Constituency
- Ward
- Cabinet
- Parliamentary Committee
- Court Case
- Company
- Organization
- Policy
- Bill
- Vote
- Government Project
- Political Promise
- Manifesto
- Award
- Honor
- Investigation
- Timeline
- Quote

---

# Guiding Principle

Everything in the system is connected.

The Kenya Political Archive is not a collection of web pages.

It is a political knowledge graph.

Person references Source

Person has Media

Person is related to another Person

## Note: Everything in the system is connected.
