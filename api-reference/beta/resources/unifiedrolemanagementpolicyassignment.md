---
title: Tipo de recurso unifiedRoleManagementPolicyAssignment
description: Um unifiedRoleManagementPolicyAssignment atribui a política a um escopo específico e à definição de função.
author: shauliu1
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c674e35692e472ea24a5670ff40950647e8d076d
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2021
ms.locfileid: "58454203"
---
# <a name="unifiedrolemanagementpolicyassignment-resource-type"></a>Tipo de recurso unifiedRoleManagementPolicyAssignment

Um unifiedRoleManagementPolicyAssignment atribui a política a um escopo específico e à definição de função.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedRoleManagementPolicyAssignments](../api/unifiedrolemanagementpolicyassignment-list.md)|[Coleção unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md)|Obter uma lista dos [objetos unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) e suas propriedades.|
|[Obter unifiedRoleManagementPolicyAssignment](../api/unifiedrolemanagementpolicyassignment-get.md)|[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md)|Leia as propriedades e as relações de [um objeto unifiedRoleManagementPolicyAssignment.](../resources/unifiedrolemanagementpolicyassignment.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo da atribuição de política.|
|policyId|Cadeia de caracteres|A id da política.|
|roleDefinitionId|Cadeia de caracteres|A id da definição de função em que a política se aplica. Se não for especificada, a política se aplicará a todas as funções.|
|scopeId|Cadeia de caracteres|A id do escopo em que a política é atribuída. Por exemplo "/", groupId, etc.|
|scopeType|Cadeia de caracteres|O tipo do escopo em que a política é atribuída. Um de Directory, DirectoryRole, Group.|

## <a name="relationships"></a>Relacionamentos
|Relação|Tipo|Descrição|
|:---|:---|:---|
|política|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)|A política da atribuição.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyAssignment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyAssignment",
  "id": "String (identifier)",
  "policyId": "String",
  "scopeId": "String",
  "scopeType": "String",
  "roleDefinitionId": "String"
}
```

