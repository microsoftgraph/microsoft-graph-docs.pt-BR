---
title: Tipo de recurso unifiedRoleManagementPolicyAssignment
description: A atribuição de uma política de gerenciamento de função a um objeto de definição de função.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b03374daa233ca550e10faefc92b1b7d7c843e5b
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247207"
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
|id|Cadeia de caracteres|Identificador exclusivo para a atribuição de política. A ID normalmente é uma concatenação da ID **unifiedRoleManagementPolicy** e **da roleDefinitionId** separadas por um sublinhado.|
|policyId|Cadeia de caracteres|A ID da política. Herdado da [entidade](../resources/entity.md).|
|roleDefinitionId|String|O identificador do objeto [de definição de](unifiedroledefinition.md) função em que a política se aplica. Se não for especificada, a política se aplicará a todas as funções. Dá suporte $filter (`eq`).|
|Scopeid|Cadeia de caracteres|O identificador do escopo em que a política é atribuída.  Pode ser para `/` o locatário ou uma ID de grupo. Obrigatório.|
|scopeType|String|O tipo do escopo em que a política é atribuída. Um dos`Directory`. `DirectoryRole` Obrigatório.|

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

