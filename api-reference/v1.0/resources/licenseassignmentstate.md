---
title: Tipo de recurso licenseAssignmentState
description: A **propriedade licenseAssignmentStates** da entidade do usuário é uma coleção de **objetos licenseAssignmentState.** Ele fornece detalhes sobre atribuições de licença para um usuário.
author: dkershaw10
ms.localizationpriority: medium
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 40dc8e13240cbeb1fe21bbaabcab38247cee25d2
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/19/2021
ms.locfileid: "60493190"
---
# <a name="licenseassignmentstate-resource-type"></a>Tipo de recurso licenseAssignmentState

Namespace: microsoft.graph


A **propriedade licenseAssignmentStates** da entidade [do](user.md) usuário é uma coleção de **objetos licenseAssignmentState.** Ele fornece detalhes sobre atribuições de licença para um usuário. Os detalhes incluem informações como:  

- Quais planos estão desabilitados para um usuário
- Se a licença foi atribuída ao usuário diretamente ou herdada de um grupo
- O estado atual da atribuição
- Detalhes de erro se o estado da atribuição for Error 


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|assignedByGroup|string|A id do grupo que atribui essa licença. Se a atribuição for uma licença atribuída diretamente, esse campo será Null. Somente Leitura.|
|disabledPlans|Collection(String)|Os planos de serviço que estão desabilitados nesta atribuição. Somente Leitura.|
|erro|Cadeia de caracteres|Erro de falha de atribuição de licença. Se a licença for atribuída com êxito, esse campo será Null. Somente Leitura. Valores possíveis: `CountViolation` , , , , e `MutuallyExclusiveViolation` `DependencyViolation` `ProhibitedInUsageLocationViolation` `UniquenessViolation` `Others` . Para obter mais informações sobre como identificar e resolver erros de atribuição de licença, [consulte aqui](/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).|
|lastUpdatedDateTime|DateTimeOffset|O timestamp quando o estado da atribuição de licença foi atualizado pela última vez.|
|skuId|Cadeia de caracteres|O identificador exclusivo da SKU. Somente Leitura.|
|state|Cadeia de caracteres|Indique o estado atual dessa atribuição. Somente Leitura. Valores possíveis: Active, ActiveWithError, Disabled e Error.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

```json
{
  "assignedByGroup": "String",
  "disabledPlans": "Collection(String)",
  "error": " String ",  
  "lastUpdatedDateTime": "String (timestamp)",
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
