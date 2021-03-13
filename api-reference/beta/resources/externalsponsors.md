---
title: tipo complexo externalSponsors
description: Identifica uma relação com outro usuário no locatário que será permitido como aprovador.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 361ac6ff85d5b4462b39aa10e4f978ce7d486e40
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761867"
---
# <a name="externalsponsors-complex-type"></a>tipo complexo externalSponsors

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado no estágio de aprovação de uma política de atribuição [de pacote de acesso.](accesspackageassignmentpolicy.md) É um subtipo de [userSet](userset.md), no qual o valor indica que os patrocinadores externos de uma organização conectada do usuário solicitante devem `@odata.type` ser o `#microsoft.graph.externalSponsors` aprovador. Esse aprovador só se aplica a solicitações de usuários que fazem parte de uma organização conectada.  Ao criar um estágio de aprovação da política de atribuição de pacote de acesso com externalSponsors, inclua também outro aprovador, como um único usuário ou membro do grupo, caso a organização conectada não tenha um patrocinador externo.

## <a name="properties"></a>Propriedades

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| isBackup | Boolean | Indica se o patrocinador é um aprovador de fallback de backup. |

## <a name="json-representation"></a>Representação JSON

A seguir está uma representação JSON desse tipo.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalSponsors",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "@odata.type": "#microsoft.graph.externalSponsors",
  "isBackup": false
}
```



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalSponsor complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


