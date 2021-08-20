---
title: Tipo de recurso office365GroupsActivityGroupCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: b7f38f2279e7cd575972d13ea411d972349131a4fe3a9943c4e5efa03365ffa2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178707"
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
| reportPeriod      | Cadeia de caracteres | O número de dias que o relatório aborda.    |

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


