---
title: tipo de recurso licenseAssignmentState
description: 'A propriedade **licenseAssignmentStates** da entidade User é uma coleção de **licenseAssignmentState**. Ele fornece detalhes sobre as atribuições de licença a um usuário. Os detalhes incluem informações como:  '
localization_priority: Normal
ms.openlocfilehash: e720070c4c97c58fd3c99e49656d7ca33f5fb9d4
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778422"
---
# <a name="licenseassignmentstate-resource-type"></a>tipo de recurso licenseAssignmentState

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A propriedade **licenseAssignmentStates** da entidade [User](user.md) é uma coleção de **licenseAssignmentState**. Ele fornece detalhes sobre as atribuições de licença a um usuário. Os detalhes incluem informações como:  

- Quais planos estão desabilitados para um usuário
- Se a licença foi atribuída ao usuário diretamente ou herdada de um grupo
- Estado atual da atribuição
- Se o estado da atribuição for erro, qual é o detalhe do erro para a falha? 


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|assignedByGroup|string|A ID do grupo que atribui essa licença. Se a atribuição for uma licença atribuída diretamente, esse campo será nulo. Somente Leitura.|
|disabledPlans|Collection(String)|Os planos de serviço que estão desabilitados nesta atribuição. Somente Leitura.|
|erro|String|Erro de falha na atribuição de licença. Se a licença for atribuída com êxito, este campo será nulo. Somente Leitura. Valores possíveis: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation` `ProhibitedInUsageLocationViolation` `UniquenessViolation`,, e `Others`. Para obter mais informações sobre como identificar e resolver erros de atribuição de licença, confira [aqui](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).|
|skuId|String|O identificador exclusivo da SKU. Somente Leitura.|
|state|String|Indica o estado atual desta atribuição. Somente Leitura. Valores possíveis: Active, ActiveWithError, Disabled e Error.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.licenseAssignmentState"
}-->
```json
{
  "assignedByGroup": "String",
  "disabledPlans": ["string"],
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```
