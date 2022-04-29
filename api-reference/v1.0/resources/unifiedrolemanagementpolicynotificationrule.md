---
title: Tipo de recurso unifiedRoleManagementPolicyNotificationRule
description: Um tipo derivado do tipo de recurso unifiedRoleManagementPolicyRule que define as regras de notificação por email para atribuições de função, ativações e aprovações.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0fae65ed41efb482278af0d3a802c9002b242891
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133845"
---
# <a name="unifiedrolemanagementpolicynotificationrule-resource-type"></a>Tipo de recurso unifiedRoleManagementPolicyNotificationRule

Namespace: microsoft.graph

Um tipo derivado do tipo de recurso [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) que define as regras de notificação por email para atribuições de função, ativações e aprovações.

Herda [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).

## <a name="methods"></a>Métodos

Nenhum.


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador da regra. Herdado da [entidade](../resources/entity.md).|
|isDefaultRecipientsEnabled|Booliano|Indica se um destinatário padrão receberá o email de notificação.|
|Notificationlevel|Cadeia de caracteres|O nível de notificação. Os valores possíveis são `None`, `Critical`. `All`|
|notificationRecipients|Coleção de cadeias de caracteres|A lista de destinatários das notificações por email.|
|Notificationtype|Cadeia de caracteres|O tipo de notificação. Há `Email` suporte apenas para isso.|
|recipientType|Cadeia de caracteres|O tipo de destinatário da notificação. Os valores possíveis são `Requestor`, `Approver`. `Admin`|
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

