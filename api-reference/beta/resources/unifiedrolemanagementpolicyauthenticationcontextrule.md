---
title: Tipo de recurso unifiedRoleManagementPolicyAuthenticationContextRule
description: Uma unifiedRoleManagementPolicyAuthenticationContextRule especifica a regra de habilitação associada a uma política de gerenciamento de função. Ele é derivado de microsoft.graph.unifiedRoleManagementPolicyRule.
author: shauliu1
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 847b3155f27b82aa616bb6471c7152f988fa000c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59046453"
---
# <a name="unifiedrolemanagementpolicyauthenticationcontextrule-resource-type"></a>Tipo de recurso unifiedRoleManagementPolicyAuthenticationContextRule

Namespace: microsoft.graph

Uma unifiedRoleManagementPolicyAuthenticationContextRule especifica a regra de habilitação associada a uma política de gerenciamento de função. Ele é derivado de microsoft.graph.unifiedRoleManagementPolicyRule.

Herda [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|claimValue|Cadeia de Caracteres|Valor da declaração de contexto de autenticação.|
|id|Cadeia de caracteres|Identificador exclusivo da regra. Herdado [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|
|isEnabled|Booliano|Indica se a configuração está habilitada.|
|destino|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|O destino da regra. Herdado [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyAuthenticationContextRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyAuthenticationContextRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "isEnabled": "Boolean",
  "claimValue": "String"
}
```

