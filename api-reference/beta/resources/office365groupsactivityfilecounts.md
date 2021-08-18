---
title: Tipo de recurso office365GroupsActivityFileCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: f05cf16e1b2e0273aaa62241bbeac3b0d872bf87605e2c852ac2ab28e25f9526
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54160860"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a>Tipo de recurso office365GroupsActivityFileCounts

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   | Descrição                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Data   | A data mais recente do conteúdo.          |
| total             | Int64  | O número total de arquivos na biblioteca de documentos SharePoint do grupo. |
| active            | Int64  | O número de arquivos que foram exibidos, editados, compartilhados ou sincronizados na biblioteca de documentos SharePoint do grupo. |
| reportDate        | Data   | A data em que vários arquivos estavam ativos no site de SharePoint do grupo. |
| reportPeriod      | Cadeia de caracteres | O número de dias que o relatório aborda.    |

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


