---
title: Tipo de recurso accessReviewInstanceDecisionItemUserTarget
description: Representa o destino de uma revisão como um usuário.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 73fba5b7329a6dd13ddc455b9ba327467dde9016
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133466"
---
# <a name="accessreviewinstancedecisionitemusertarget-resource-type"></a>Tipo de recurso accessReviewInstanceDecisionItemUserTarget

Namespace: microsoft.graph

Representa uma identidade de usuário sob revisão em [um accessReviewInstance](accessreviewinstance.md).

Herda de [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).

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
