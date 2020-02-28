---
title: tipo complexo Únicousuário
description: Identifica um usuário no locatário que será permitido como solicitante, Aprovador ou revisor.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0d4db47278051dd79b697dc352549b95b872e4aa
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331338"
---
# <a name="singleuser-complex-type"></a>tipo complexo Únicousuário

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado nas configurações de solicitação, aprovação e revisão de atribuição de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md). O `@odata.type` valor `#microsoft.graph.singleUser` indica que este conjunto de usuários identifica um usuário específico no locatário que será permitido como solicitante, Aprovador ou revisor.

## <a name="properties"></a>Propriedades

Este tipo tem as seguintes propriedades:

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| id |Cadeia de caracteres | A ID do usuário no Azure AD. |
| descrição |String | O nome do usuário no Azure AD. Somente leitura. |
| IsBackup | Booliano | Para um **únicousuário** em um estágio de aprovação, indica se o usuário é um Aprovador de fallback de backup. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do tipo.

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
