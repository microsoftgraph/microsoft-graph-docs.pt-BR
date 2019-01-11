---
title: tipo de recurso de office365GroupsActivityStorage
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 9824d3d172a8578f8a25a049c2d0d3b407bbc47e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862248"
---
# <a name="office365groupsactivitystorage-resource-type"></a>tipo de recurso de office365GroupsActivityStorage

## <a name="properties"></a>Propriedades

| Propriedade                  | Tipo   | Descrição                              |
| :------------------------ | :----- | ---------------------------------------- |
| reportRefreshDate         | Data   | A última data do conteúdo.          |
| mailboxStorageUsedInBytes | Int64  | O armazenamento utilizado na caixa de correio de grupo.       |
| siteStorageUsedInBytes    | Int64  | O armazenamento usado na biblioteca de documentos do SharePoint. |
| reportDate                | Data   | A data de instantâneo do Exchange e SharePoint usou o armazenamento. |
| reportPeriod              | Cadeia de caracteres | O número de dias que abrange o relatório.    |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "mailboxStorageUsedInBytes": 1024, 
  "siteStorageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
