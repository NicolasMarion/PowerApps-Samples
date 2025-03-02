# Export and import a data map

This sample shows how to create an import map (data map) in Dynamics 365, export it as an XML formatted data, import modified mappings, and create a new import map in Dynamics 365 based on the imported mappings.

## How to run this sample

See [How to run samples](../../../README.md) for information about how to run this sample.

## What this sample does

The `BulkDeleteRequest` message is intended to be used in a scenario where it contains data that is needed to create the bulk delete request.

## How this sample works

In order to simulate the scenario described in [What this sample does](#what-this-sample-does), the sample will do the following:

### Setup

1. Checks for the current version of the org.
2. The `CreateImportMapping` method creates the import mapping record.
3. The `RetrieveMappingXML` method exports the mapping that is created.
4. The `ChangeMappingName` method parse the xml to change the name attribute.

### Clean up

1. Display an option to delete the sample data that is created in [Setup](#setup).

    The deletion is optional in case you want to examine the entities and data created by the sample. You can manually delete the records to achieve the same result.
