---
title: tipo complexo singleUser
description: Identifica um usuário no locatário que será permitido como solicitante, aprovador ou revisor.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8e1982eef048e1f68f579df7f2ebc6b0975f2f0b
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761041"
---
# <a name="singleuser-complex-type"></a>tipo complexo singleUser

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado nas configurações de solicitação, aprovação e revisão de atribuição de uma política de atribuição [de pacote de acesso.](accesspackageassignmentpolicy.md) O valor indica que esse conjunto de usuários identifica um usuário específico no locatário que será permitido como  `@odata.type` `#microsoft.graph.singleUser` solicitante, aprovador ou revisor.

## <a name="properties"></a>Propriedades

Esse tipo tem as seguintes propriedades:

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| id |Cadeia de caracteres | A ID do usuário no Azure AD. |
| descrição |Cadeia de caracteres | O nome do usuário no Azure AD. Somente leitura. |
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
  "id": "string (identifier)",
  "description": "string"
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


