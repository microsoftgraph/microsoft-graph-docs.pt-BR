---
title: Tipo de recurso unifiedRoleManagementPolicyNotificationRule
description: Um unifiedRoleManagementPolicyNotificationRule especifica a regra de notificação associada a uma política de gerenciamento de função. Ele é derivado de microsoft.graph.unifiedRoleManagementPolicyRule.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e4d8952f8ab69ed83aecde96f3bc2804affe24c8
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299095"
---
# <a name="unifiedrolemanagementpolicynotificationrule-resource-type"></a>Tipo de recurso unifiedRoleManagementPolicyNotificationRule

Namespace: microsoft.graph

Um unifiedRoleManagementPolicyNotificationRule especifica a regra de notificação associada a uma política de gerenciamento de função. Ele é derivado de microsoft.graph.unifiedRoleManagementPolicyRule.

Herda [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo da regra. Herdado [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|
|notificationLevel|Cadeia de caracteres|O nível de notificação. Um de Nenhum, Crítico, Todos.|
|notificationRecipients|Coleção de cadeias de caracteres|A lista de recepients de notificação como email.|
|notificationType|Cadeia de caracteres|O tipo de notificação. Um de Email.|
|recipientType|Cadeia de caracteres|O tipo de destinatário. Um dos Solicitadores, Aprovadores, Administradores.|
|isDefaultRecipientsEnabled|Booliano|Se o destinatário padrão está recebendo o email ou não.|
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

