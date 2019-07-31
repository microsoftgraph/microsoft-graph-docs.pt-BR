---
title: tipo de recurso office365GroupsActivityFileCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 8154f24fe36f2c11f3926412c3fcc062be04b5ef
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966521"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a>tipo de recurso office365GroupsActivityFileCounts

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   | Descrição                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Data   | A última data do conteúdo.          |
| total             | Int64  | O número total de arquivos na biblioteca de documentos do SharePoint do grupo. |
| active            | Int64  | O número de arquivos que foram exibidos, editados, compartilhados ou sincronizados na biblioteca de documentos do SharePoint do grupo. |
| reportDate        | Data   | A data em que um número de arquivos estava ativo no site do SharePoint do grupo. |
| reportPeriod      | String | O número de dias que o relatório cobre.    |

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
