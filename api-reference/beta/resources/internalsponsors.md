---
title: tipo complexo internalSponsors
description: Identifica uma relação com outro usuário no locatário que será permitido como Aprovador.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e556daf6fd8039b6783c6d08e595d0df1a6c3541
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42495407"
---
# <a name="internalsponsors-complex-type"></a>tipo complexo internalSponsors

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usada no estágio de aprovação de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md). É um subtipo de [userset](userset.md), no qual o valor `@odata.type` `#microsoft.graph.internalSponsors` indica que os patrocinadores internos da organização conectada do usuário solicitante sejam o aprovador. Esse aprovador só é aplicável a solicitações de usuários que fazem parte de uma organização conectada.  Ao criar um estágio de aprovação de política de atribuição de pacote do Access com o internalSponsors, também inclua outro aprovador, como um único usuário ou membro de grupo, caso a organização conectada não tenha um patrocinador interno.

## <a name="properties"></a>Propriedades

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| IsBackup | Boolean | Indica se o patrocinador é um Aprovador de fallback de backup. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do tipo.

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
