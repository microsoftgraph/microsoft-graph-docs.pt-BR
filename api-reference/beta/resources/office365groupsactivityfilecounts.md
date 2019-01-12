---
title: tipo de recurso de office365GroupsActivityFileCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: adff009d9047aa147c8042059fbdab8491288fb7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972555"
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
