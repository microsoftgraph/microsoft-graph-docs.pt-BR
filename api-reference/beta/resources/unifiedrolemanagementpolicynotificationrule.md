---
title: Tipo de recurso unifiedRoleManagementPolicyNotificationRule
description: Um tipo derivado do tipo de recurso unifiedRoleManagementPolicyRule que define as regras de notificação por email para atribuições de função, ativações e aprovações.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a7f70afe8daa0bd296033be244bf2f7370ce1bdd
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65898536"
---
# <a name="unifiedrolemanagementpolicynotificationrule-resource-type"></a>Tipo de recurso unifiedRoleManagementPolicyNotificationRule

Namespace: microsoft.graph

Um tipo derivado do tipo de recurso [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) que define as regras de notificação por email para atribuições de função, ativações e aprovações.

Herda [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador da regra. Herdado da [entidade](../resources/entity.md).|
|isDefaultRecipientsEnabled|Booliano|Indica se um destinatário padrão receberá o email de notificação.|
|Notificationlevel|Cadeia de Caracteres|O nível de notificação. Os valores possíveis são `None`, `Critical`. `All`|
|notificationRecipients|Coleção de cadeias de caracteres|A lista de destinatários das notificações por email.|
|Notificationtype|Cadeia de Caracteres|O tipo de notificação. Há `Email` suporte apenas para isso.|
|recipientType|String|O tipo de destinatário da notificação. Os valores possíveis são `Requestor`, `Approver`. `Admin`|
|destino|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|Define detalhes do escopo direcionado pela regra de notificação. Os detalhes podem incluir o tipo de entidade de segurança, o tipo de atribuição de função e as ações que afetam uma função. Herdado [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md). Suporta `$filter` (`eq`, `ne`).|

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
  "isDefaultRecipientsEnabled": "Boolean",
  "notificationRecipients": [
    "String"
  ]
}
```