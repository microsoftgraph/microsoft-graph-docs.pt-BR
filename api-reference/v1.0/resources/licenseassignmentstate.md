---
title: tipo de recurso licenseAssignmentState
description: A propriedade **licenseAssignmentStates** da entidade User é uma coleção de objetos **licenseAssignmentState** . Ele fornece detalhes sobre as atribuições de licença a um usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: b26ab4be63cbb40929dbea3f40522ee4c6b7ff70
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/17/2020
ms.locfileid: "48582181"
---
# <a name="licenseassignmentstate-resource-type"></a>tipo de recurso licenseAssignmentState

Namespace: microsoft.graph


A propriedade **licenseAssignmentStates** da entidade [User](user.md) é uma coleção de objetos **licenseAssignmentState** . Ele fornece detalhes sobre as atribuições de licença a um usuário. Os detalhes incluem informações como:  

- Quais planos estão desabilitados para um usuário
- Se a licença foi atribuída ao usuário diretamente ou herdada de um grupo
- O estado atual da atribuição
- Detalhes do erro se o estado da atribuição for erro 


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|assignedByGroup|cadeia de caracteres|A ID do grupo que atribui essa licença. Se a atribuição for uma licença atribuída diretamente, esse campo será nulo. Somente Leitura.|
|disabledPlans|Collection(String)|Os planos de serviço que estão desabilitados nesta atribuição. Somente Leitura.|
|erro|String|Erro de falha na atribuição de licença. Se a licença for atribuída com êxito, este campo será nulo. Somente Leitura. Valores possíveis: `CountViolation` , `MutuallyExclusiveViolation` ,,, `DependencyViolation` `ProhibitedInUsageLocationViolation` `UniquenessViolation` e `Others` . Para obter mais informações sobre como identificar e resolver erros de atribuição de licença, confira [aqui](/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).|
|skuId|String|O identificador exclusivo da SKU. Somente Leitura.|
|state|String|Indica o estado atual desta atribuição. Somente Leitura. Valores possíveis: Active, ActiveWithError, Disabled e Error.|

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