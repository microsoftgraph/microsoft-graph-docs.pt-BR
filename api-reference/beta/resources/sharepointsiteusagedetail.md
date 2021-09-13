---
title: Tipo de recurso sharePointSiteUsageDetail
description: Veja a seguir uma representação JSON do recurso.
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 2d9bdd86d2b50601dc5c54b2a34480e9cd71118d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59038794"
---
# <a name="sharepointsiteusagedetail-resource-type"></a>Tipo de recurso sharePointSiteUsageDetail

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade                | Tipo    |
| :---------------------- | :------ |
| reportRefreshDate       | Data    |
| siteId                  | Guid  |
| siteUrl                 | Cadeia de Caracteres  |
| ownerDisplayName        | Cadeia de Caracteres  |
| ownerPrincipalName      | Cadeia de Caracteres  |
| isDeleted               | Boleano |
| lastActivityDate        | Data    |
| siteSensitivityLabelId  | Cadeia de Caracteres  |
| externalSharing         | Boleano |
| unmanagedDevicePolicy   | Cadeia de Caracteres  |
| geoLocation             | Cadeia de Caracteres  |
| fileCount               | Int64   |
| activeFileCount         | Int64   |
| pageViewCount           | Int64   |
| visitPageCount        | Int64   |
| anonymousLinkCount      | Int64   |
| companyLinkCount        | Int64   |
| secureLinkForGuestCount | Int64   |
| secureLinkForMemberCount| Int64   |
| storageUsedInBytes      | Int64   |
| storageAllocatedInBytes | Int64   |
| rootWebTemplate         | Cadeia de Caracteres  |
| reportPeriod            | Cadeia de Caracteres  |

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
  "siteSensitivityLabelId": "String",
  "externalSharing": true,
  "unmanagedDevicePolicy": "String",
  "geoLocation": "String",
  "fileCount": 1024,
  "activeFileCount": 1024,
  "pageViewCount": 1024,
  "visitedPageCount": 1024,
  "anonymousLinkCount": 5,
  "companyLinkCount": 8,
  "secureLinkForGuestCount": 13,
  "secureLinkForMemberCount": 11,
  "storageUsedInBytes": 1024,
  "storageAllocatedInBytes": 1024,
  "rootWebTemplate": "String",
  "reportPeriod": "String"
}
```


