---
languages:
- csharp
products:
- power-platform
page_type: sample
description: "Sample to audit user access."
---

# Audit User Access

This sample code shows how to audit user access. 

## How to run this sample

See [How to run samples](../../../README.md) for information about how to run this sample.

## What this sample does

This sample first enables user access auditing with the logged on user's organization. Next, it creates and modifies an account entity so that audit records are generated.

## How this sample works

In order to simulate the scenario described in [What this sample does](#what-this-sample-does), the sample will do the following:

### Setup

1. Checks for the current version of the org.
1. Creates a new account entity and enables auditing on the new account entity.

### Demonstrate

1. Gets the organization's ID from the system user record and retrieves organization record.
2. Enables auditing on the organization, including auditing for user access.
3. Makes an update request ti the account entity to be tracked by auditing.
4. set the organization and account auditing flags back to old values and retrieve them if they were actually changed.

### Clean up

1. Display an option to delete the records created during [Setup](#setup). 

    The deletion is optional in case you want to examine the entities and data created by the sample. You can manually delete the records to achieve the same result.
