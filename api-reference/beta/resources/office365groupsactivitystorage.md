---
title: tipo de recurso de office365GroupsActivityStorage
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0485fd95046bc83350983bc1333dba83c79139d6
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576378"
---
# <a name="office365groupsactivitystorage-resource-type"></a>tipo de recurso de office365GroupsActivityStorage

## <a name="properties"></a>Propriedades

| Propriedade                  | Tipo   | Descrição                              |
| :------------------------ | :----- | ---------------------------------------- |
| reportRefreshDate         | Data   | A última data do conteúdo.          |
| mailboxStorageUsedInBytes | Int64  | O armazenamento utilizado na caixa de correio de grupo.       |
| siteStorageUsedInBytes    | Int64  | O armazenamento usado na biblioteca de documentos do SharePoint. |
| reportDate                | Data   | A data de instantâneo do Exchange e SharePoint usou o armazenamento. |
| reportPeriod              | String | O número de dias que abrange o relatório.    |

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
