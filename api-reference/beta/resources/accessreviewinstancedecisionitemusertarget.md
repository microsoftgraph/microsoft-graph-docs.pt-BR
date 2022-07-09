---
title: Tipo de recurso accessReviewInstanceDecisionItemUserTarget
description: Representa o destino de uma revisão como um usuário.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f64e29f3b1ef13471147be495dcd100e80742304
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698125"
---
# <a name="accessreviewinstancedecisionitemusertarget-resource-type"></a>Tipo de recurso accessReviewInstanceDecisionItemUserTarget

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Representa uma identidade de usuário em revisão em [um accessReviewInstance](accessreviewinstance.md).

Herda de [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| userDisplayName | Cadeia de caracteres | O nome do usuário. |
| userId | Cadeia de caracteres | O identificador do usuário. |
| userPrincipalName | Cadeia de caracteres | O nome da entidade de segurança do usuário. |

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
