---
title: Tipo de recurso unifiedRoleManagementPolicy
description: Um unifiedRoleManagementPolicy especifica as várias políticas associadas a um escopo e uma definição de função. Ele é derivado de microsoft.graph.policyBase.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a4d53873710269c68501b8cdd3201ae71083e015
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461335"
---
# <a name="unifiedrolemanagementpolicy-resource-type"></a>Tipo de recurso unifiedRoleManagementPolicy

Namespace: microsoft.graph

Um unifiedRoleManagementPolicy especifica as várias políticas associadas a um escopo Azure AD definição de função. Ele é derivado da [entidade](entity.md). Para políticas que se aplicam ao RBAC do Azure, use a [API REST PIM do Azure para políticas de gerenciamento de funções](/rest/api/authorization/role-management-policies).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedRoleManagementPolicies](../api/policyroot-list-rolemanagementpolicies.md)|[Coleção unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)|Obtenha uma lista dos [objetos unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) e suas propriedades.|
|[Obter unifiedRoleManagementPolicy](../api/unifiedrolemanagementpolicy-get.md)|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)|Leia as propriedades e as relações de um [objeto unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) considerando o escopo.|
|[Listar regras](../api/unifiedrolemanagementpolicy-list-rules.md)|[Coleção unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Obtenha os recursos unifiedRoleManagementPolicyRule da propriedade de navegação de regras.|
|[Obter regras](../api/unifiedrolemanagementpolicyrule-get.md)|[Coleção unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Obtenha as regras para um objeto unifiedRoleManagementPolicyRule.|
|[Atualizar regras](../api/unifiedrolemanagementpolicyrule-update.md)|[Coleção unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Atualize as regras para um objeto unifiedRoleManagementPolicyRule.|
<!--unsurface effectiveRules because it hasn't been implemented
|[List effectiveRules](../api/unifiedrolemanagementpolicy-list-effectiverules.md)|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) collection|Get the unifiedRoleManagementPolicyRule resources from the effectiveRules navigation property.|
-->

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|String|Descrição da política.|
|displayName|String|Nome de exibição da política.|
|id|String|Identificador exclusivo da política.|
|isOrganizationDefault|Booliano|Isso só pode ser definido como true para uma única política de todo o locatário que será aplicada a todos os escopos e funções. Defina scopeId como "/" e scopeType como Directory.|
|lastModifiedBy|[identity](../resources/identity.md)|A identidade que modificou a configuração de função pela última vez.|
|lastModifiedDateTime|DateTimeOffset|A hora em que a configuração de função foi modificada pela última vez.|
|Scopeid|String|A ID do escopo em que a política é criada. Pode ser para `/` o locatário ou uma ID de grupo. Obrigatório.|
|scopeType|String|O tipo do escopo em que a política é criada. Um dos`Directory`. `DirectoryRole` Obrigatório.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|effectiveRules|[Coleção unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|**Não implementado.** A lista de regras efetivas, como regras de aprovação e regras de expiração avaliadas com base em regras referenciadas herdadas. Por exemplo, se houver uma política em todo o locatário para impor a habilitação de uma regra de aprovação, a regra efetiva será habilitar a aprovação mesmo que a política tenha uma regra para desabilitar a aprovação.|
|Regras|[Coleção unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|A coleção de regras, como regras de aprovação e regras de expiração.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicy",
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

