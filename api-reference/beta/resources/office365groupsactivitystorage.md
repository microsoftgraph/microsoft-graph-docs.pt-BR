---
title: tipo de recurso office365GroupsActivityStorage
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0485fd95046bc83350983bc1333dba83c79139d6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32505547"
---
# <a name="office365groupsactivitystorage-resource-type"></a>tipo de recurso office365GroupsActivityStorage

## <a name="properties"></a>Propriedades

| Propriedade                  | Tipo   | Descrição                              |
| :------------------------ | :----- | ---------------------------------------- |
| reportRefreshDate         | Data   | A última data do conteúdo.          |
| mailboxStorageUsedInBytes | Int64  | O armazenamento usado na caixa de correio de grupo.       |
| siteStorageUsedInBytes    | Int64  | O armazenamento usado na biblioteca de documentos do SharePoint. |
| reportDate                | Data   | A data do instantâneo para o armazenamento usado pelo Exchange e pelo SharePoint. |
| reportPeriod              | String | O número de dias que o relatório cobre.    |

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
