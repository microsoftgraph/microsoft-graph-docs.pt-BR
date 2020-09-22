---
title: tipo de recurso office365GroupsActivityStorage
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 0b14e6981a193ad1698303d2762d0321de430b73
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092388"
---
# <a name="office365groupsactivitystorage-resource-type"></a>tipo de recurso office365GroupsActivityStorage

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade                  | Tipo   | Descrição                              |
| :------------------------ | :----- | ---------------------------------------- |
| reportRefreshDate         | Data   | A última data do conteúdo.          |
| mailboxStorageUsedInBytes | Int64  | O armazenamento usado na caixa de correio de grupo.       |
| siteStorageUsedInBytes    | Int64  | O armazenamento usado na biblioteca de documentos do SharePoint. |
| reportDate                | Data   | A data do instantâneo para o armazenamento usado pelo Exchange e pelo SharePoint. |
| reportPeriod              | Cadeia de caracteres | O número de dias que o relatório cobre.    |

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


