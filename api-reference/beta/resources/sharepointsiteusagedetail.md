---
title: Tipo de recurso sharePointSiteUsageDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: d52d7675521c297ee602102847ddb3fa653d3d8af3efba64f3a71d783d83a708
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54176173"
---
# <a name="sharepointsiteusagedetail-resource-type"></a>Tipo de recurso sharePointSiteUsageDetail

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade                | Tipo    |
| :---------------------- | :------ |
| reportRefreshDate       | Data    |
| siteId                  | Guid  |
| siteUrl                 | Cadeia de caracteres  |
| ownerDisplayName        | Cadeia de caracteres  |
| ownerPrincipalName      | Cadeia de caracteres  |
| isDeleted               | Boolean |
| lastActivityDate        | Data    |
| SiteSensitivityLabelId  | Cadeia de caracteres  |
| ExternalSharing         | Boolean |
| UnmanagedDevicePolicy   | Cadeia de caracteres  |
| GeoLocation             | Cadeia de caracteres  |
| fileCount               | Int64   |
| activeFileCount         | Int64   |
| pageViewCount           | Int64   |
| visitPageCount        | Int64   |
| AnonymousLinkCount      | Int64   |
| CompanyLinkCount        | Int64   |
| SecureLinkForGuestCount | Int64   |
| SecureLinkForMemberCount| Int64   |
| storageUsedInBytes      | Int64   |
| storageAllocatedInBytes | Int64   |
| rootWebTemplate         | Cadeia de caracteres  |
| reportPeriod            | Cadeia de caracteres  |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointSiteUsageDetail"
} -->

```json
{
  "reportRefreshDate": "Date",
  "siteId": "Guid",
  "siteUrl": "String",
  "ownerDisplayName": "String",
  "ownerPrincipalName": "String",
  "isDeleted": true,
  "lastActivityDate": "Date",
  "lastActivityDate": "2017-09-01", 
  "SiteSensitivityLabelId": "String",
  "ExternalSharing": true,
  "UnmanagedDevicePolicy": "String",
  "GeoLocation": "String",
  "fileCount": 1024,
  "activeFileCount": 1024,
  "pageViewCount": 1024,
  "visitedPageCount": 1024,
  "AnonymousLinkCount": 5,
  "CompanyLinkCount": 8,
  "SecureLinkForGuestCount": 13,
  "SecureLinkForMemberCount": 11,
  "storageUsedInBytes": 1024,
  "storageAllocatedInBytes": 1024,
  "rootWebTemplate": "String",
  "reportPeriod": "String"
}
```


