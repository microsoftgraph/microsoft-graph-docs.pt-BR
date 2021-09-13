---
title: Tipo de recurso unifiedRoleManagementPolicy
description: Um unifiedRoleManagementPolicy especifica as várias políticas associadas a um escopo e uma definição de função. Ele é derivado de microsoft.graph.policyBase.
author: shauliu1
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b27726e12815f058091bc09308344c150cb73b2f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59046516"
---
# <a name="unifiedrolemanagementpolicy-resource-type"></a>Tipo de recurso unifiedRoleManagementPolicy

Namespace: microsoft.graph

Um unifiedRoleManagementPolicy especifica as várias políticas associadas a um escopo e uma definição de função. Ele é derivado de microsoft.graph.policyBase.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedRoleManagementPolicies](../api/unifiedrolemanagementpolicy-list.md)|[Coleção unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)|Obter uma lista dos [objetos unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) e suas propriedades.|
|[Obter unifiedRoleManagementPolicy](../api/unifiedrolemanagementpolicy-get.md)|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)|Leia as propriedades e as relações de [um objeto unifiedRoleManagementPolicy.](../resources/unifiedrolemanagementpolicy.md)|
|[Listar effectiveRules](../api/unifiedrolemanagementpolicy-list-effectiverules.md)|[Coleção unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Obter os recursos unifiedRoleManagementPolicyRule da propriedade de navegação effectiveRules.|
|[Listar regras](../api/unifiedrolemanagementpolicy-list-rules.md)|[Coleção unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Obter os recursos unifiedRoleManagementPolicyRule da propriedade de navegação de regras.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|description|Cadeia de caracteres|Descrição da política.|
|displayName|Cadeia de caracteres|Nome de exibição da política.|
|id|Cadeia de caracteres|Identificador exclusivo da política.|
|isOrganizationDefault|Boleano|Isso só pode ser definido como true para uma única política de toda a locatário que se aplicará a todos os escopos e funções. De definir o scopeId como "/" e scopeType como Directory.|
|lastModifiedBy|[identity](../resources/identity.md)|A identidade que modificou a configuração da função pela última vez.|
|lastModifiedDateTime|DateTimeOffset|A hora em que a configuração da função foi modificada pela última vez.|
|scopeId|Cadeia de Caracteres|A id do escopo em que a política é criada. Por exemplo "/", groupId, etc.|
|scopeType|Cadeia de Caracteres|O tipo do escopo em que a política é criada. Um de Directory, DirectoryRole, Group.|

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

