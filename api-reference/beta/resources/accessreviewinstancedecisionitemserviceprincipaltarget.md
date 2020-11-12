---
title: tipo de recurso accessReviewInstanceDecisionItemServicePrincipalTarget
description: Representa o destino de uma revisão como um destino principal de serviço.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e9943a287dd28a44f3b36eae1a92d1b2c385496c
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000778"
---
# <a name="accessreviewinstancedecisionitemserviceprincipaltarget-resource-type"></a>tipo de recurso accessReviewInstanceDecisionItemServicePrincipalTarget

Namespace: microsoft.graph

Representa uma entidade de serviço em revisão em um [accessReviewInstance](accessreviewinstance.md).

Herda de [accessReviewInstanceDecisionItemTarget](../resources/accessreviewinstancedecisionitemtarget.md).

## <a name="properties"></a>Propriedades
| Propriedade | Tipo | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| servicePrincipalName | Cadeia de caracteres | O identificador da entidade de serviço cujo acesso está sendo revisado. |
| servicePrincipalDisplayName | Cadeia de caracteres | O nome de exibição da entidade de serviço cujo acesso está sendo revisado. |
| appId | Cadeia de caracteres | A appId da entidade de segurança de serviço que está sendo revisada. |

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
