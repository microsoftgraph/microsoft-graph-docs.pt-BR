---
title: Tipo de recurso unifiedRoleManagementPolicyNotificationRule
description: Um unifiedRoleManagementPolicyNotificationRule especifica a regra de notificação associada a uma política de gerenciamento de função. Ele é derivado de microsoft.graph.unifiedRoleManagementPolicyRule.
author: shauliu1
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: eae130fb4fdf2781aa8cb8a83d6cdd03314bb1fd
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59074484"
---
# <a name="unifiedrolemanagementpolicynotificationrule-resource-type"></a>Tipo de recurso unifiedRoleManagementPolicyNotificationRule

Namespace: microsoft.graph

Um unifiedRoleManagementPolicyNotificationRule especifica a regra de notificação associada a uma política de gerenciamento de função. Ele é derivado de microsoft.graph.unifiedRoleManagementPolicyRule.

Herda [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo da regra. Herdado [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|
|notificationLevel|String|O nível de notificação. Um de Nenhum, Crítico, Todos.|
|notificationRecipients|String collection|A lista de recepients de notificação como email.|
|notificationType|String|O tipo de notificação. Um de Email.|
|recipientType|Cadeia de Caracteres|O tipo de destinatário. Um dos Solicitadores, Aprovadores, Administradores.|
|isDefaultRecipientsEnabled|Boolean|Se o destinatário padrão está recebendo o email ou não.|
|destino|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|O destino da regra. Herdado [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "notificationType": "String",
  "recipientType": "String",
  "notificationLevel": "String",
  "isDefaultRecipientsEnabled": true,
  "notificationRecipients": [
    "String"
  ]
}
```

