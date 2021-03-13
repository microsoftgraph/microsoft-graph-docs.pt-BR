---
title: Tipo complexo internalSponsors
description: Identifica uma relação com outro usuário no locatário que será permitido como aprovador.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 84c53bbeacde51afc88f5c0b4b5c13bc4f68b430
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760894"
---
# <a name="internalsponsors-complex-type"></a>Tipo complexo internalSponsors

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado no estágio de aprovação de uma política de atribuição [de pacote de acesso.](accesspackageassignmentpolicy.md) É um subtipo de [userSet](userset.md), no qual o valor indica que os patrocinadores internos da organização conectada de um usuário solicitante devem `@odata.type` ser o `#microsoft.graph.internalSponsors` aprovador. Esse aprovador só se aplica a solicitações de usuários que fazem parte de uma organização conectada.  Ao criar um estágio de aprovação da política de atribuição de pacote de acesso com internalSponsors, inclua também outro aprovador, como um único usuário ou membro do grupo, caso a organização conectada não tenha um patrocinador interno.

## <a name="properties"></a>Propriedades

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| isBackup | Boolean | Indica se o patrocinador é um aprovador de fallback de backup. |

## <a name="json-representation"></a>Representação JSON

A seguir está uma representação JSON do tipo.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.internalSponsors",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "@odata.type": "#microsoft.graph.internalSponsors",
  "isBackup": false
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "internalSponsor complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


