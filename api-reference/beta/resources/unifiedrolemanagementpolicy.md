---
title: Tipo de recurso unifiedRoleManagementPolicy
description: Especifica as várias políticas associadas a escopos e funções.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d1c97cb00b3ef6f3ac8a6b8d2588706f421571f6
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899096"
---
# <a name="unifiedrolemanagementpolicy-resource-type"></a>Tipo de recurso unifiedRoleManagementPolicy

Namespace: microsoft.graph

Especifica as várias políticas associadas a escopos e funções. Para políticas que se aplicam ao RBAC do Azure, use a [API REST PIM do Azure para políticas de gerenciamento de funções](/rest/api/authorization/role-management-policies).

Atualmente, todas as políticas e regras associadas são somente leitura.

Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedRoleManagementPolicies](../api/policyroot-list-rolemanagementpolicies.md)|[Coleção unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)|Obtenha políticas de gerenciamento de funções e seus detalhes.|
|[Obter unifiedRoleManagementPolicy](../api/unifiedrolemanagementpolicy-get.md)|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)|Recupere os detalhes de uma política de gerenciamento de função.|
|[Listar regras](../api/unifiedrolemanagementpolicy-list-rules.md)|[Coleção unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Obter as regras definidas para uma política de gerenciamento de função.|
|[Obter unifiedRoleManagementPolicyRule](../api/unifiedrolemanagementpolicyrule-get.md)|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Recuperar uma regra definida para uma política de gerenciamento de função.|


## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|String|Descrição da política.|
|displayName|String|Nome de exibição da política.|
|id|String|Identificador exclusivo da política.|
|isOrganizationDefault|Booliano|Isso só pode ser definido para `true` uma única política de todo o locatário que será aplicada a todos os escopos e funções. Defina scopeId como `/` e scopeType como `Directory`. Suporta `$filter` (`eq`, `ne`).|
|lastModifiedBy|[identity](../resources/identity.md)|A identidade que modificou a configuração de função pela última vez.|
|lastModifiedDateTime|DateTimeOffset|A hora em que a configuração de função foi modificada pela última vez.|
|Scopeid|Cadeia de Caracteres|O identificador do escopo em que a política é criada. Pode ser para `/` o locatário ou uma ID de grupo. Obrigatório.|
|scopeType|Cadeia de Caracteres|O tipo do escopo em que a política é criada. Um dos`Directory`. `DirectoryRole` Obrigatório.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|effectiveRules|[Coleção unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)| A lista de regras efetivas, como regras de aprovação e regras de expiração avaliadas com base em regras referenciadas herdadas. Por exemplo, se houver uma política em todo o locatário para impor a habilitação de uma regra de aprovação, a regra efetiva será habilitar a aprovação mesmo que a política tenha uma regra para desabilitar a aprovação. Suporta o `$expand`.|
|Regras|[Coleção unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|A coleção de regras, como regras de aprovação e regras de expiração. Suporta o `$expand`.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "isOrganizationDefault": "Boolean",
  "scopeId": "String",
  "scopeType": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identity"
  }
}
```
