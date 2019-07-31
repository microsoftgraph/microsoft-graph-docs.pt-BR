---
title: tipo de recurso office365GroupsActivityStorage
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: a3168ad417f246017ba1018aca265ec0363c951e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009458"
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
