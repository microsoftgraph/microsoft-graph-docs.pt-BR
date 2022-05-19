---
title: Tipo de recurso licenseAssignmentState
description: 'A **propriedade licenseAssignmentStates** da entidade de usuário é uma coleção **de licenseAssignmentState**. Ele fornece detalhes sobre atribuições de licença para um usuário. Os detalhes incluem informações como:  '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: users
author: jconley76
ms.openlocfilehash: 266e85843aaa7fada2c0e7bd00946ae3e0a6886b
ms.sourcegitcommit: 562dc670cea411de0ecc232840ce1c650abbe34c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2022
ms.locfileid: "65549565"
---
# <a name="licenseassignmentstate-resource-type"></a>Tipo de recurso licenseAssignmentState

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A **propriedade licenseAssignmentStates** da entidade [de](user.md) usuário é uma coleção **de licenseAssignmentState**. Ele fornece detalhes sobre atribuições de licença para um usuário. Os detalhes incluem informações como:

- Quais planos estão desabilitados para um usuário
- Se a licença foi atribuída ao usuário diretamente ou herdada de um grupo
- Estado atual da atribuição
- Se o estado da atribuição for Erro, qual é o detalhe do erro para a falha?


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|assignedByGroup|string|A ID do grupo que atribui essa licença. Se a atribuição for uma licença atribuída direta, esse campo será Nulo. Somente Leitura.|
|disabledPlans|Collection(String)|Os planos de serviço que estão desabilitados nesta atribuição. Somente Leitura.|
|erro|Cadeia de caracteres|Erro de falha de atribuição de licença. Se a licença for atribuída com êxito, esse campo será Nulo. Somente Leitura. Os valores possíveis são `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`e `UniquenessViolation``Other`. Para obter mais informações sobre como identificar e resolver erros de atribuição de licença, [consulte aqui](/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).|
|lastUpdatedDateTime|DateTimeOffset|O carimbo de data/hora em que o estado da atribuição de licença foi atualizado pela última vez.|
|skuId|String|O identificador exclusivo da SKU. Somente Leitura.|
|state|Cadeia de caracteres|Indique o estado atual dessa atribuição. Somente Leitura. Os valores possíveis são `Active`, `ActiveWithError`, `Disabled` e `Error`.|

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
  "lastUpdatedDateTime": "String (timestamp)",
  "skuId": " String ",
  "state": "String"
}

```
