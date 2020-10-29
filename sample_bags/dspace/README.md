The bags in this directory were created with DSpace 6.3 using the Replication Task Suite. Each bag represents an object
which can be found in a DSpace repository, e.g. Community, and are named according to how they are found within DSpace.

Each bag stores metadata about the DSpace object (e.g. roles, authorizations) in the form of xml and bitstreams for
any binary content held by the object.

Expectations for the bags are as follows:
* SITE@123456789-0 - The DSpace Site, contains metadata about the repository and its contents
* COMMUNITY@123456789-1 - The top level Community in the exported repository, contains metadata
* COLLECTION@123456789-2 - A Collection which exists in the Community, contains metadata
* ITEM@123456789-3 - An Item stored under the Collection, contains metadata and bitstreams for the Item.
