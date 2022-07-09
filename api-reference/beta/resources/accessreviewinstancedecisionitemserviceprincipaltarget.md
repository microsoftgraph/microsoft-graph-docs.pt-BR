---
title: Tipo de recurso accessReviewInstanceDecisionItemServicePrincipalTarget
description: Representa o destino de uma revisão como um destino de entidade de serviço.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: dafb1cde55fe510edcff89bd5497997d136a12a9
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698139"
---
# <a name="accessreviewinstancedecisionitemserviceprincipaltarget-resource-type"></a>Tipo de recurso accessReviewInstanceDecisionItemServicePrincipalTarget

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Representa uma entidade de serviço em revisão em [um accessReviewInstance](accessreviewinstance.md).

Herda de [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).

## <a name="properties"></a>Propriedades
| Propriedade | Tipo | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| servicePrincipalID | Cadeia de caracteres | O identificador da entidade de serviço cujo acesso está sendo revisado. |
| servicePrincipalDisplayName | Cadeia de caracteres | O nome de exibição da entidade de serviço cujo acesso está sendo revisado. |
| appId | Cadeia de caracteres | A appId da entidade de entidade de serviço que está sendo revisada. |

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
