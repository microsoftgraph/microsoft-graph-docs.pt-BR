---
title: Tipo de recurso unifiedRoleManagementPolicyAssignment
description: A atribuição de uma política de gerenciamento de função a um objeto de definição de função.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 813e0bd3ec6c5327f3bd0028d9b1c8c59eab5c5d
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133901"
---
# <a name="unifiedrolemanagementpolicyassignment-resource-type"></a>Tipo de recurso unifiedRoleManagementPolicyAssignment

Namespace: microsoft.graph

A atribuição de uma política de gerenciamento de função a um [objeto de definição de](../resources/unifiedroledefinition.md) função.

Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedRoleManagementPolicyAssignments](../api/policyroot-list-rolemanagementpolicyassignments.md)|[Coleção unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md)|Obtenha uma lista dos [objetos unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) e suas propriedades.|
|[Obter unifiedRoleManagementPolicyAssignment](../api/unifiedrolemanagementpolicyassignment-get.md)|[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md)|Leia as propriedades e as relações de um [objeto unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) .|

<!--
|[Create unifiedRoleManagementPolicyAssignment](../api/policyroot-post-rolemanagementpolicyassignments.md)|[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md)|Create a new [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) object.|
|[Update unifiedRoleManagementPolicyAssignment](../api/unifiedrolemanagementpolicyassignment-update.md)|[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md)|Update the properties of an [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) object.|
|[Delete unifiedRoleManagementPolicyAssignment](../api/unifiedrolemanagementpolicyassignment-delete.md)|None|Deletes an [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) object.|
|[List unifiedRoleManagementPolicy](../api/unifiedrolemanagementpolicyassignment-list-policy.md)|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) collection|Get the unifiedRoleManagementPolicy resources from the policy navigation property.|
|[Add unifiedRoleManagementPolicy](../api/unifiedrolemanagementpolicyassignment-post-policy.md)|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)|Add policy by posting to the policy collection.|
-->

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo para a atribuição de política. A ID normalmente é uma concatenação da ID **unifiedRoleManagementPolicy** e **da roleDefinitionId** separadas por um sublinhado.|
|policyId|Cadeia de caracteres|A ID da política. Herdado da [entidade](../resources/entity.md).|
|roleDefinitionId|Cadeia de caracteres|O identificador do objeto [de definição de](unifiedroledefinition.md) função em que a política se aplica. Se não for especificada, a política se aplicará a todas as funções. Dá suporte $filter (`eq`).|
|Scopeid|Cadeia de caracteres|O identificador do escopo em que a política é atribuída.  Pode ser para `/` o locatário ou uma ID de grupo. Obrigatório.|
|scopeType|Cadeia de caracteres|O tipo do escopo em que a política é atribuída. Um dos`Directory`. `DirectoryRole` Obrigatório.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|política|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)| A política associada a uma atribuição de política. Dá `$expand` suporte e um aninhado `$expand` das **regras e** **das relações effectiveRules** para a política.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyAssignment",
  "baseType": "microsoft.graph.entity",
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

