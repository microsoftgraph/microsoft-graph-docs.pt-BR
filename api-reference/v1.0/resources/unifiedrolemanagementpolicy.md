---
title: Tipo de recurso unifiedRoleManagementPolicy
description: Especifica as várias políticas associadas a escopos e funções.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3e9ce46b44b5e21d326c6c751ae7f6553a2c2199
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2022
ms.locfileid: "65246920"
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
|[Atualizar unifiedRoleManagementPolicyRule](../api/unifiedrolemanagementpolicyrule-get.md)|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Atualize uma regra definida para uma política de gerenciamento de função.|


## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|Cadeia de caracteres|Descrição da política.|
|displayName|Cadeia de caracteres|Nome de exibição da política.|
|id|String|Identificador exclusivo da política.|
|isOrganizationDefault|Booliano|Isso só pode ser definido para `true` uma única política de todo o locatário que será aplicada a todos os escopos e funções. Defina scopeId como `/` e scopeType como `Directory`. Suporta `$filter` (`eq`, `ne`).|
|lastModifiedBy|[identity](../resources/identity.md)|A identidade que modificou a configuração de função pela última vez.|
|lastModifiedDateTime|DateTimeOffset|A hora em que a configuração de função foi modificada pela última vez.|
|Scopeid|String|O identificador do escopo em que a política é criada. Pode ser para `/` o locatário ou uma ID de grupo. Obrigatório.|
|scopeType|String|O tipo do escopo em que a política é criada. Um dos`Directory`. `DirectoryRole` Obrigatório.|

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

