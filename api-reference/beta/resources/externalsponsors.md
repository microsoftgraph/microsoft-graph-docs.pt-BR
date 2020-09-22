---
title: tipo complexo externalSponsors
description: Identifica uma relação com outro usuário no locatário que será permitido como Aprovador.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4db88b74ae0acb2e817bd575f4e990774533064e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013690"
---
# <a name="externalsponsors-complex-type"></a>tipo complexo externalSponsors

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usada no estágio de aprovação de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md). É um subtipo de [userset](userset.md), no qual o `@odata.type` valor `#microsoft.graph.externalSponsors` indica que os patrocinadores externos da organização conectada do usuário solicitante sejam o aprovador. Esse aprovador só é aplicável a solicitações de usuários que fazem parte de uma organização conectada.  Ao criar um estágio de aprovação de política de atribuição de pacote do Access com o externalSponsors, também inclua outro aprovador, como um único usuário ou membro de grupo, caso a organização conectada não tenha um patrocinador externo.

## <a name="properties"></a>Propriedades

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| IsBackup | Booliano | Indica se o patrocinador é um Aprovador de fallback de backup. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON desse tipo.

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


