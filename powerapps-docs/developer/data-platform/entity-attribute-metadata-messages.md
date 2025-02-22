---
title: "Table column definitions messages (Microsoft Dataverse) | Microsoft Docs" # Intent and product brand in a unique string of 43-59 chars including spaces
description: "About the messages used to edit table column definitions, also known as properties or columns." # 115-145 characters including spaces. This abstract displays in the search result.
ms.date: 06/15/2022
ms.reviewer: jdaly
ms.topic: article
author: NHelgren # GitHub ID
ms.subservice: dataverse-developer
ms.author: nhelgren # MSFT alias of Microsoft employees only
search.audienceType: 
  - developer
---
# Table column definitions messages

A column is a container for a piece of data in a table. The term *attribute* and *property* (class property) are often used interchangeably with the term *table column*. Model-driven apps use the term *column* when they refer to table columns.  

[!INCLUDE[cc-terminology](includes/cc-terminology.md)]

## Table column messages
 
The following table lists the messages that you can use to perform actions on table columns.  
  
|Message|Web API Operation|SDK Assembly|
|-------------|-----------------|-----------------|  
|`CreateAttribute`</br></br>Create table columns|POST to EntityMetadata Attributes collection-valued navigation property with JSON definition of column. More information: [Create columns](webapi/create-update-column-definitions-using-web-api.md#create-columns)|<xref:Microsoft.Xrm.Sdk.Messages.CreateAttributeRequest>|
|`DeleteAttribute`</br></br>Delete table columns|DELETE to the URL of the column.|<xref:Microsoft.Xrm.Sdk.Messages.DeleteAttributeRequest>|  
|`DeleteOptionValue`</br></br>Delete a choice from <xref:Microsoft.Xrm.Sdk.Metadata.PicklistAttributeMetadata> or <xref:Microsoft.Xrm.Sdk.Metadata.StatusAttributeMetadata> columns|<xref:Microsoft.Dynamics.CRM.DeleteOptionValue?text=DeleteOptionValue Action>|<xref:Microsoft.Xrm.Sdk.Messages.DeleteOptionValueRequest>|
|`InsertOptionValue`</br></br>Add a choice to a <xref:Microsoft.Xrm.Sdk.Metadata.PicklistAttributeMetadata> column|<xref:Microsoft.Dynamics.CRM.InsertOptionValue?text=InsertOptionValue Action" />|<xref:Microsoft.Xrm.Sdk.Messages.InsertOptionValueRequest>|
|`InsertStatusValue`</br></br>Add a choice to a <xref:Microsoft.Xrm.Sdk.Metadata.StatusAttributeMetadata> column|<xref:Microsoft.Dynamics.CRM.InsertStatusValue?text=InsertStatusValue Action>|<xref:Microsoft.Xrm.Sdk.Messages.InsertStatusValueRequest>|  
|`OrderOption`</br></br>Changes the order of the choice presented in an <xref:Microsoft.Xrm.Sdk.Metadata.PicklistAttributeMetadata> column|<xref:Microsoft.Dynamics.CRM.OrderOption?text=OrderOption Action>|<xref:Microsoft.Xrm.Sdk.Messages.OrderOptionRequest>|
|`RetrieveAttribute`</br></br>Retrieve a table column|Use the Web API query mentioned in [Querying EntityMetadata columns](webapi/query-metadata-web-api.md#bkmk_queryAttributesexample) to retrieve table columns.|<xref:Microsoft.Xrm.Sdk.Messages.RetrieveAttributeRequest>|  
|`UpdateAttribute`</br></br>Update a table column|See [Update tables](webapi/create-update-entity-definitions-using-web-api.md#update-table-definitions)|<xref:Microsoft.Xrm.Sdk.Messages.UpdateAttributeRequest>|  
|`UpdateStateValue`</br></br>Update the label for a <xref:Microsoft.Xrm.Sdk.Metadata.StateAttributeMetadata> column|<xref:Microsoft.Dynamics.CRM.UpdateStateValue?text=UpdateStateValue Action>|<xref:Microsoft.Xrm.Sdk.Messages.UpdateStateValueRequest>|

### See also  

[Column definitions](entity-attribute-metadata.md)<br />
[Create auto-number column](create-auto-number-attributes.md)<br />
[Work with columns definitions](org-service/samples/work-with-attributes.md)<br />
[Sample: Dump column definitions information to a file](org-service/samples/dump-attribute-metadata.md)

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
