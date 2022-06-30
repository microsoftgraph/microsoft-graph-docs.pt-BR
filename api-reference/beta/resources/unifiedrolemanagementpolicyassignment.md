---
title: Tipo de recurso unifiedRoleManagementPolicyAssignment
description: Um unifiedRoleManagementPolicyAssignment atribui a política a um escopo e definição de função específicos.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8dfbe842f6e60abec9c0f15881695062e901d5ba
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446312"
---
# <a name="unifiedrolemanagementpolicyassignment-resource-type"></a>Tipo de recurso unifiedRoleManagementPolicyAssignment

Namespace: microsoft.graph

A atribuição de uma política de gerenciamento de função a um [objeto de definição de](../resources/unifiedroledefinition.md) função.

Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedRoleManagementPolicyAssignments](../api/policyroot-list-rolemanagementpolicyassignments.md)|[Coleção unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md)|Obtenha os detalhes de todas as atribuições de política de gerenciamento de função, incluindo as políticas e as regras associadas à Azure AD função.|
|[Obter unifiedRoleManagementPolicyAssignment](../api/unifiedrolemanagementpolicyassignment-get.md)|[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md)|Leia as propriedades e as relações de um [objeto unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo para a atribuição de política. A ID normalmente é uma concatenação da ID unifiedRoleManagementPolicy e da roleDefinitionId separadas por um sublinhado.|
|policyId|String|A ID da política. Herdado da [entidade](../resources/entity.md).|
|roleDefinitionId|String|O identificador do objeto [de definição de](unifiedroledefinition.md) função em que a política se aplica. Se não for especificada, a política se aplicará a todas as funções. Dá suporte $filter (`eq`).|
|Scopeid|Cadeia de caracteres|O identificador do escopo em que a política é atribuída.  Pode ser para `/` o locatário ou uma ID de grupo. Obrigatório.|
|scopeType|String|O tipo do escopo em que a política é atribuída. Um dos`Directory`. `DirectoryRole` Obrigatório.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|política|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)|A política associada a uma atribuição de política. Dá $expand e a um $expand das regras e das relações effectiveRules para a política.|

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

