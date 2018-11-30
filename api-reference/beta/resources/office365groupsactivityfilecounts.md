---
title: tipo de recurso de office365GroupsActivityFileCounts
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: eb2d967108d4f75064b91670ae43fb7a2dd7ce7a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034332"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a>tipo de recurso de office365GroupsActivityFileCounts

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   | Descrição                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Data   | A última data do conteúdo.          |
| total             | Int64  | O número total de arquivos na biblioteca de documentos do SharePoint do grupo. |
| ativo            | Int64  | O número de arquivos que foram exibidos, editado, compartilhados ou sincronizados na biblioteca de documentos do SharePoint do grupo. |
| reportDate        | Data   | A data em que um número de arquivos foram ativo no site do SharePoint do grupo. |
| reportPeriod      | String | O número de dias que abrange o relatório.    |

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
