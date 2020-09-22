---
title: tipo de recurso office365GroupsActivityGroupCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: c249123a01cde2fe952f5111affe645415ddc6cc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092381"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a>tipo de recurso office365GroupsActivityGroupCounts

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   | Descrição                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Data   | A última data do conteúdo.          |
| total             | Int64  | O número total de grupos.              |
| active            | Int64  | O número de grupos ativos. Um grupo é considerado ativo se qualquer um dos seguintes ocorrerem: caixa de correio de grupo recebidas emails; arquivos de usuário exibidos, editados, compartilhados ou sincronizados na biblioteca de documentos do SharePoint; páginas do SharePoint exibidas pelo usuário; mensagens postadas, lidas ou curtidas pelo usuário em grupos do Yammer. |
| reportDate        | Data   | A data em que um número de grupos estava ativo. |
| reportPeriod      | Cadeia de caracteres | O número de dias que o relatório cobre.    |

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


