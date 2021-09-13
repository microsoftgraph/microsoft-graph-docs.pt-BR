---
title: Tipo de recurso office365GroupsActivityFileCounts
description: Veja a seguir uma representação JSON do recurso.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 0c7d2b89dde8e288fb8ca81dc7ca67e6830a4122
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59142828"
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
| reportPeriod      | Cadeia de Caracteres | O número de dias que o relatório aborda.    |

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


