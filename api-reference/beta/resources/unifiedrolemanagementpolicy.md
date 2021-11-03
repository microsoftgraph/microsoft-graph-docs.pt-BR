---
title: Tipo de recurso unifiedRoleManagementPolicy
description: Um unifiedRoleManagementPolicy especifica as várias políticas associadas a um escopo e uma definição de função. Ele é derivado de microsoft.graph.policyBase.
author: carolinetempleton
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 4680bc93bed7995eb35d08ecf4d10750710ca40e
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687533"
---
# <a name="unifiedrolemanagementpolicy-resource-type"></a>Tipo de recurso unifiedRoleManagementPolicy

Namespace: microsoft.graph

Um unifiedRoleManagementPolicy especifica as várias políticas associadas a um escopo e uma definição de função. Ele é derivado de microsoft.graph.policyBase.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedRoleManagementPolicies](../api/unifiedrolemanagementpolicy-list.md)|[Coleção unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)|Obter uma lista dos [objetos unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) e suas propriedades.|
|[Obter unifiedRoleManagementPolicy](../api/unifiedrolemanagementpolicy-get.md)|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)|Leia as propriedades e as relações de [um objeto unifiedRoleManagementPolicy.](../resources/unifiedrolemanagementpolicy.md)|
|[Listar effectiveRules](../api/unifiedrolemanagementpolicy-list-effectiverules.md)|[Coleção unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Obter os recursos unifiedRoleManagementPolicyRule da propriedade de navegação effectiveRules.|
|[Listar regras](../api/unifiedrolemanagementpolicy-list-rules.md)|[Coleção unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Obter os recursos unifiedRoleManagementPolicyRule da propriedade de navegação de regras.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|String|Descrição da política.|
|displayName|String|Nome de exibição da política.|
|id|String|Identificador exclusivo da política.|
|isOrganizationDefault|Booliano|Isso só pode ser definido como true para uma única política de toda a locatário que se aplicará a todos os escopos e funções. De definir o scopeId como "/" e scopeType como Directory.|
|lastModifiedBy|[identity](../resources/identity.md)|A identidade que modificou a configuração da função pela última vez.|
|lastModifiedDateTime|DateTimeOffset|A hora em que a configuração da função foi modificada pela última vez.|
|scopeId|String|A id do escopo em que a política é criada. Por exemplo "/", groupId, etc.|
|scopeType|String|O tipo do escopo em que a política é criada. Um de Directory, DirectoryRole, Group.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|effectiveRules|[Coleção unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|A lista de regras efetivas, como regra de aprovação, regra de expiração, etc. avaliada com base em regras referenciadas herdadas. Por exemplo Se houver uma política de todo o locatário para impor a regra de aprovação de habilitação, a regra efetiva será habilitar a aprovação, mesmo que a política tenha uma regra para desabilitar a aprovação.|
|rules|[Coleção unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|A coleção de regras, como regra de aprovação, regra de expiração, etc.|

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

