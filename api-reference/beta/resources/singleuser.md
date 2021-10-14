---
title: tipo complexo singleUser
description: Identifica um usuário no locatário que será permitido como solicitante, aprovador ou revisor.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e7ccc22478a470047e6f65387419bfc0364bf548
ms.sourcegitcommit: f4999aa6fc05f845027db01aa489f7086f9850e1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/13/2021
ms.locfileid: "60290243"
---
# <a name="singleuser-complex-type"></a>tipo complexo singleUser

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado nas configurações de solicitação, aprovação e revisão de atribuição de uma política de atribuição [de pacote de acesso.](accesspackageassignmentpolicy.md) O valor indica que esse userSet identifica um usuário específico no locatário que será permitido como  `@odata.type` `#microsoft.graph.singleUser` solicitante, aprovador ou revisor.

## <a name="properties"></a>Propriedades

Esse tipo tem as seguintes propriedades:

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| id |String | A ID do usuário no Azure AD. |
| description |String | O nome do usuário no Azure AD. Somente leitura. |
| isBackup | Boolean | Para um **singleUser** em um estágio de aprovação, indica se o usuário é um aprovador de fallback de backup. |

## <a name="json-representation"></a>Representação JSON

A seguir está uma representação JSON do tipo.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.singleUser",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "isBackup": false,
  "id": "String (identifier)",
  "description": "String"
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "singleUser complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


