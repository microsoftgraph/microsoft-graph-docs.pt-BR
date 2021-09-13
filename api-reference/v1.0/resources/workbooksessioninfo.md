---
title: Tipo de recurso workbookSessionInfo
description: Fornece informações sobre a sessão de pasta de trabalho.
author: lumine2008
ms.localizationpriority: medium
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 47c3fbe839b5e5f17e76217ca2cda633d8c42c6a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134133"
---
# <a name="workbooksessioninfo-resource-type"></a>Tipo de recurso workbookSessionInfo

Namespace: microsoft.graph

Fornece informações sobre a sessão de pasta de trabalho.


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.workbookSessionInfo"
}-->

```json
{
  "id": "string",
  "persistChanges": true
}
```

## <a name="properties"></a>Propriedades

| Propriedade | Tipo  | Descrição                               |
|:---------|:------|:------------------------------------------|
| id  | cadeia de caracteres | ID da sessão de pasta de trabalho. |
| persistChanges | booliano |  `true` para sessão persistente. `false` para sessão não persistente (modo de exibição) |


