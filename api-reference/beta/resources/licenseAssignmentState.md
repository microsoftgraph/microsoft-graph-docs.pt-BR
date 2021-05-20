---
title: Tipo de recurso licenseAssignmentState
description: 'A **propriedade licenseAssignmentStates** da entidade do usuário é uma coleção **de licenseAssignmentState**. Ele fornece detalhes sobre atribuições de licença para um usuário. Os detalhes incluem informações como:  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: jpettere
ms.openlocfilehash: 06b469cb80e92ca09a8e1bce7a058aed1b3a570d
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547075"
---
# <a name="licenseassignmentstate-resource-type"></a>Tipo de recurso licenseAssignmentState

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A **propriedade licenseAssignmentStates** da entidade [do](user.md) usuário é uma coleção **de licenseAssignmentState**. Ele fornece detalhes sobre atribuições de licença para um usuário. Os detalhes incluem informações como:

- Quais planos estão desabilitados para um usuário
- Se a licença foi atribuída ao usuário diretamente ou herdada de um grupo
- Estado atual da atribuição
- Se o estado da atribuição for Error, qual é o detalhe de erro da falha?


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|assignedByGroup|cadeia de caracteres|A id do grupo que atribui essa licença. Se a atribuição for uma licença atribuída diretamente, esse campo será Null. Somente Leitura.|
|disabledPlans|Collection(String)|Os planos de serviço que estão desabilitados nesta atribuição. Somente Leitura.|
|erro|String|Erro de falha de atribuição de licença. Se a licença for atribuída com êxito, esse campo será Null. Somente Leitura. Valores possíveis: `CountViolation` , , , , e `MutuallyExclusiveViolation` `DependencyViolation` `ProhibitedInUsageLocationViolation` `UniquenessViolation` `Others` . Para obter mais informações sobre como identificar e resolver erros de atribuição de licença, [consulte aqui](/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).|
|skuId|String|O identificador exclusivo da SKU. Somente Leitura.|
|state|String|Indique o estado atual dessa atribuição. Somente Leitura. Valores possíveis: Active, ActiveWithError, Disabled e Error.|

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