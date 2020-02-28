---
title: tipo complexo requestorManager
description: Identifica uma relação com outro usuário no locatário que será permitido como Aprovador.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b7eea64e2d3f1d32b7ca60fc0c3a548401f7ef23
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331336"
---
# <a name="requestomanager-complex-type"></a>tipo complexo requestoManager

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado nas configurações de aprovação de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md). É um subtipo de [userset](userset.md), no qual o `@odata.type` valor `#microsoft.graph.requestorManager` indica que o gerente de um usuário solicitante é o aprovador.  Ao criar um estágio de aprovação de política de atribuição de pacote do Access com o requestorManager, também inclua outro aprovador, como um único usuário ou membro de grupo, caso o usuário solicitante não tenha um gerente.


## <a name="properties"></a>Propriedades


| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| IsBackup | Booliano | Para um gerente em um estágio de aprovação, indica se o gerente é um Aprovador de fallback de backup. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do tipo.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestorManager",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "isBackup": false
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "requestorManager complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
