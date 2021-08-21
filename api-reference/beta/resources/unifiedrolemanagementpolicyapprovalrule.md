---
title: Tipo de recurso unifiedRoleManagementPolicyApprovalRule
description: Um unifiedRoleManagementPolicyApprovalRule especifica a regra de aprovação associada a uma política de gerenciamento de função. Ele é derivado de microsoft.graph.unifiedRoleManagementPolicyRule.
author: shauliu1
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e2c28045bb0e5882d8ee9d8c000d0e6b8a48657a
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453818"
---
# <a name="unifiedrolemanagementpolicyapprovalrule-resource-type"></a>Tipo de recurso unifiedRoleManagementPolicyApprovalRule

Namespace: microsoft.graph

Um unifiedRoleManagementPolicyApprovalRule especifica a regra de aprovação associada a uma política de gerenciamento de função. Ele é derivado de microsoft.graph.unifiedRoleManagementPolicyRule.

Herda [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo da regra. Herdado [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|
|configuração|[approvalSettings](../resources/approvalsettings.md)|A configuração de aprovação da regra.|
|destino|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|O destino da regra. Herdado [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyApprovalRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyApprovalRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "setting": {
    "@odata.type": "microsoft.graph.approvalSettings"
  }
}
```

