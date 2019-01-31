---
title: tipo de recurso de licenseAssignmentState
description: A propriedade **licenseAssignmentStates** da entidade do usuário é uma coleção de objetos **licenseAssignmentState** . Ela fornece detalhes sobre as atribuições de licença a um usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 0822c975ab81badf5334881bb460532161858010
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29649365"
---
# <a name="licenseassignmentstate-resource-type"></a>tipo de recurso de licenseAssignmentState


A propriedade **licenseAssignmentStates** da entidade do [usuário](user.md) é uma coleção de objetos **licenseAssignmentState** . Ela fornece detalhes sobre as atribuições de licença a um usuário. Os detalhes incluem informações como:  

 - Quais planos estão desabilitados para um usuário
 - Se a licença foi atribuída ao usuário diretamente ou herdada de um grupo
 - O estado atual da atribuição
 - Detalhes do erro se o estado de atribuição for erro 


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|assignedByGroup|cadeia de caracteres|A identificação do grupo que atribui essa licença. Se a atribuição for uma licença atribuído diretamente, esse campo será Null. Somente Leitura.|
|disabledPlans|Collection(String)|Os planos de serviço que serão desabilitados nessa atribuição. Somente Leitura.|
|erro|String|Erro de falha de atribuição de licença. Se a licença foi distribuída com êxito, esse campo será Null. Somente Leitura. Valores possíveis: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, e `Others`. Para obter mais informações sobre como identificar e resolver a atribuição de licença erros consulte [aqui](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).|
|skuId|String|O identificador exclusivo da SKU. Somente Leitura.|
|state|String|Indica o estado atual dessa atribuição. Somente Leitura. Valores possíveis: ativo, ActiveWithError, desabilitado e erro.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

```json
{
  "assignedByGroup": "String",
  "disabledPlans": "Collection(String)",
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseAssignmentState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: microsoft.graph.user/licenseAssignmentStates:
      Referenced type microsoft.graph.licenseAssignmentState is not defined in the doc set! Potential suggestion: UNKNOWN"
  ]
}-->
