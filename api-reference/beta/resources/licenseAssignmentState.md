---
title: Tipo de recurso licenseAssignmentState
description: 'A **propriedade licenseAssignmentStates** da entidade do usuário é uma coleção **de licenseAssignmentState**. Ele fornece detalhes sobre atribuições de licença para um usuário. Os detalhes incluem informações como:  '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: users
author: jpettere
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
|assignedByGroup|string|A id do grupo que atribui essa licença. Se a atribuição for uma licença atribuída diretamente, esse campo será Null. Somente Leitura.|
|disabledPlans|Collection(String)|Os planos de serviço que estão desabilitados nesta atribuição. Somente Leitura.|
|erro|Cadeia de caracteres|Erro de falha de atribuição de licença. Se a licença for atribuída com êxito, esse campo será Null. Somente Leitura. Os valores possíveis são `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`e `Other`. Para obter mais informações sobre como identificar e resolver erros de atribuição de licença, [consulte aqui](/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).|
|lastUpdatedDateTime|DateTimeOffset|O timestamp quando o estado da atribuição de licença foi atualizado pela última vez.|
|skuId|String|O identificador exclusivo da SKU. Somente Leitura.|
|state|String|Indique o estado atual dessa atribuição. Somente Leitura. Os valores possíveis são `Active`, `ActiveWithError`, `Disabled` e `Error`.|

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
