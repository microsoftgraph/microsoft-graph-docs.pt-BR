---
title: tipo de recurso accessReviewInstanceDecisionItemUserTarget
description: Representa o destino de uma revisão como um usuário.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: aa2117895599ba1d2c4b9829b7cad22b581f2055
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000777"
---
# <a name="accessreviewinstancedecisionitemusertarget-resource-type"></a>tipo de recurso accessReviewInstanceDecisionItemUserTarget

Namespace: microsoft.graph

Representa uma identidade de usuário em revisão em um [accessReviewInstance](accessreviewinstance.md).

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
