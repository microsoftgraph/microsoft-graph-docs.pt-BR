---
title: Tipo de recurso accessReviewInstanceDecisionItemUserTarget
description: Representa o destino de uma revisão como usuário.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f10796937aa99e5808cb51bdb4069bd99d645db2
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "51469210"
---
# <a name="accessreviewinstancedecisionitemusertarget-resource-type"></a>Tipo de recurso accessReviewInstanceDecisionItemUserTarget

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Representa uma identidade de usuário em revisão em [um accessReviewInstance](accessreviewinstance.md).

Herda [de accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| userDisplayName | Cadeia de caracteres | O nome do usuário. |
| userId | Cadeia de caracteres | O identificador do usuário. |
| userPrincipalName | String | O nome da entidade de segurança do usuário. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemUserTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String"
}
```
