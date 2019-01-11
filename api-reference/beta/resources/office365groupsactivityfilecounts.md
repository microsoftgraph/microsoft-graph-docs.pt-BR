---
title: tipo de recurso de office365GroupsActivityFileCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 856bb4c74c8af35775b6fe71cb75d89935440bdb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819180"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a>tipo de recurso de office365GroupsActivityFileCounts

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   | Descrição                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Data   | A última data do conteúdo.          |
| total             | Int64  | O número total de arquivos na biblioteca de documentos do SharePoint do grupo. |
| ativo            | Int64  | O número de arquivos que foram exibidos, editado, compartilhados ou sincronizados na biblioteca de documentos do SharePoint do grupo. |
| reportDate        | Data   | A data em que um número de arquivos foram ativo no site do SharePoint do grupo. |
| reportPeriod      | Cadeia de caracteres | O número de dias que abrange o relatório.    |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {

  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityFileCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
