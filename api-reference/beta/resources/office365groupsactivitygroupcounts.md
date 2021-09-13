---
title: Tipo de recurso office365GroupsActivityGroupCounts
description: Veja a seguir uma representação JSON do recurso.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 6548d32250d99a99f83e98d40c40041102caeb16
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59105780"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a>Tipo de recurso office365GroupsActivityGroupCounts

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   | Descrição                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Data   | A data mais recente do conteúdo.          |
| total             | Int64  | O número total de grupos.              |
| active            | Int64  | O número de grupos ativos. Um grupo será considerado ativo se ocorrer um dos seguintes: caixa de correio de grupo recebeu emails; arquivos exibidos, editados, compartilhados ou sincronizados no SharePoint de documentos; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups. |
| reportDate        | Data   | A data em que vários grupos estavam ativos. |
| reportPeriod      | Cadeia de Caracteres | O número de dias que o relatório aborda.    |

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


