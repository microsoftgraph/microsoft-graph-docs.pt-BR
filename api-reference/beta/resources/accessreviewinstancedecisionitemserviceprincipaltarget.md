---
title: Tipo de recurso accessReviewInstanceDecisionItemServicePrincipalTarget
description: Representa o destino de uma revisão como um destino de entidade de serviço.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ef944fdd1b8dbe989b1ad92e3d49b1b057fdef74
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133494"
---
# <a name="accessreviewinstancedecisionitemserviceprincipaltarget-resource-type"></a>Tipo de recurso accessReviewInstanceDecisionItemServicePrincipalTarget

Namespace: microsoft.graph

Representa uma entidade de serviço em revisão em [um accessReviewInstance](accessreviewinstance.md).

Herda de [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).

## <a name="properties"></a>Propriedades
| Propriedade | Tipo | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| servicePrincipalID | String | O identificador da entidade de serviço cujo acesso está sendo revisado. |
| servicePrincipalDisplayName | String | O nome de exibição da entidade de serviço cujo acesso está sendo revisado. |
| appId | String | A appId da entidade de entidade de serviço que está sendo revisada. |

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
