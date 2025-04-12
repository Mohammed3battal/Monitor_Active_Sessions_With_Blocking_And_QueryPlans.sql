## Script: Monitor Active User Sessions, Blocking Chains, and Executing Queries

**Description**:
This script provides a detailed, real-time report of active user sessions, including their current executing statement, blocking relationships, resource waits, isolation levels, and even query execution plans.

**What It Shows**:
- Active user session IDs and status
- Login name, host, and application name
- Blocking session ID (if blocked)
- Current command being executed
- CPU time, reads, writes, and last activity time
- Wait type and wait resource
- Transaction isolation level
- Currently executing SQL statement
- Object name involved in the execution
- Full query plan (XML format)

**Use Case**:
Use this script for:
- Diagnosing blocking or long-running queries
- Viewing real-time SQL execution and resource waits
- Gathering query plans without using Activity Monitor

**Notes**:
- Filters out system sessions and the current session
- May require `VIEW SERVER STATE` permission
- Works on SQL Server 2012 and later

**Tip**:
Wrap this query in a SQL Agent job or monitoring dashboard to track issues over time.
