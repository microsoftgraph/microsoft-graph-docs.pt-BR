---
title: Tipo de recurso office365GroupsActivityGroupCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: ad2610f5cbd3aae56651a0a5651e4ee4319b3bb2
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981491"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a>Tipo de recurso office365GroupsActivityGroupCounts

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   | Descrição                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Data   | A data mais recente do conteúdo.          |
| total             | Int64  | O número total de grupos.              |
| ativo            | Int64  | O número de grupos ativos. Um grupo será considerado ativo se ocorrer um dos seguintes: email recebido da caixa de correio do grupo; usuário visualizado, editado, compartilhado ou sincronizado arquivos na biblioteca de documentos do SharePoint; usuário visualizou páginas do SharePoint; usuário postou, leu ou curtiu mensagens em grupos do Yammer. |
| reportDate        | Data   | A data em que vários grupos estavam ativos. |
| reportPeriod      | Cadeia de caracteres | O número de dias que o relatório abrange.    |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityGroupCounts"
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


