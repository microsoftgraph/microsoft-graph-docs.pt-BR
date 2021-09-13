---
title: Tipo de recurso unifiedRoleManagementPolicyEnablementRule
description: Uma unifiedRoleManagementPolicyEnablementRule especifica a regra de habilitação associada a uma política de gerenciamento de função. Ele é derivado de microsoft.graph.unifiedRoleManagementPolicyRule.
author: shauliu1
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0919ed951b13cf1f8dcfca6aef9fc264a343f29f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59046467"
---
# <a name="unifiedrolemanagementpolicyenablementrule-resource-type"></a>Tipo de recurso unifiedRoleManagementPolicyEnablementRule

Namespace: microsoft.graph

Uma unifiedRoleManagementPolicyEnablementRule especifica a regra de habilitação associada a uma política de gerenciamento de função. Ele é derivado de microsoft.graph.unifiedRoleManagementPolicyRule.

Herda [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|enabledRules|Conjunto de cadeias de caracteres|As regras que estão habilitadas. Os valores permitidos são MultifactorAuthentication, Justification, Ticketing.|
|id|Cadeia de caracteres|Identificador exclusivo da regra. Herdado [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|
|destino|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|O destino da regra. Herdado [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyEnablementRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyEnablementRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "enabledRules": [
    "String"
  ]
}
```

