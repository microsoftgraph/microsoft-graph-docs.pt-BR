---
title: Tipo de recurso accessReviewInstanceDecisionItemServicePrincipalTarget
description: Representa o destino de uma revisão como um destino de entidade de serviço.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7d8032282d7ddaf41779b73f707b0749e3c82dd0
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "51469220"
---
# <a name="accessreviewinstancedecisionitemserviceprincipaltarget-resource-type"></a>Tipo de recurso accessReviewInstanceDecisionItemServicePrincipalTarget

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Representa uma entidade de serviço em revisão em [um accessReviewInstance](accessreviewinstance.md).

Herda [de accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).

## <a name="properties"></a>Propriedades
| Propriedade | Tipo | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| servicePrincipalID | String | O identificador da entidade de serviço cujo acesso está sendo revisado. |
| servicePrincipalDisplayName | String | O nome de exibição da entidade de serviço cujo acesso está sendo revisado. |
| appId | String | O appId da entidade principal do serviço que está sendo revisada. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemServicePrincipalTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemServicePrincipalTarget",
  "servicePrincipalId": "String",
  "servicePrincipalDisplayName": "String",
  "appId": "String"
}
```
