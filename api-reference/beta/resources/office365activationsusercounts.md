---
title: Tipo de recurso office365ActivationsUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: de01adee754940bd43be258b4454b7c68c0e4f8254581486d59a34f9a1f06478
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54139141"
---
# <a name="office365activationsusercounts-resource-type"></a>Tipo de recurso office365ActivationsUserCounts

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade                 | Tipo   | Descrição                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | Data   | A data mais recente do conteúdo.          |
| productType              | Cadeia de caracteres | O tipo de produto como "Microsoft 365 ProPlus" ou "Project Client". |
| atribuído                 | Int64  | O número de usuários que foram atribuídos à licença do produto. |
| ativado                | Int64  | O número de usuários que ativaram o produto. |
| sharedComputerActivation | Int64  | O número de usuários que usaram o produto em um computador compartilhado. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationsUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "productType": "String", 
  "assigned": 1024, 
  "activated": 1024,
  "sharedComputerActivation": 1024
}
```


