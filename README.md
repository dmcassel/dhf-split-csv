# MarkLogic Data Hub Framework CSV Splitting Flow

I found examples of using DHF ingest flows to split CSV documents on their way into the staging database, but sometimes it's more convenient to upload a full CSV to staging and then split it. This repo contains a flow with two steps:

1. Custom step to split the original CSV into individual JSON documents in the staging database
2. Mapping step map those JSON documents onto an entity and write to the final database

## Data

I'm working with data from Philadelphia's OpenDataPhilly project, specifically [CSV data showing City Landmarks][data]. 

[data]: https://www.opendataphilly.org/dataset/city-landmarks/resource/1104674f-6413-4076-97c3-a2e1f0558565
