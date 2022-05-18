---
title: Tipo de recurso unifiedRoleManagementPolicyRule
description: Um tipo abstrato que define as regras ou configurações associadas às políticas de gerenciamento de função.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 54444e25d6967536fa2e9a444fd05adf66467881
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461258"
---
# <a name="unifiedrolemanagementpolicyrule-resource-type"></a>Tipo de recurso unifiedRoleManagementPolicyRule

Namespace: microsoft.graph


Um tipo abstrato que define as regras ou configurações associadas às políticas de gerenciamento de função. Esse tipo abstrato é herdado pelos seguintes recursos que definem os vários tipos de regras e suas configurações associadas às políticas de gerenciamento de função.
+ [unifiedRoleManagementPolicyApprovalRule](unifiedrolemanagementpolicyapprovalrule.md)
+ [unifiedRoleManagementPolicyAuthenticationContextRule](unifiedrolemanagementpolicyauthenticationcontextrule.md)
+ [unifiedRoleManagementPolicyEnablementRule](unifiedrolemanagementpolicyenablementrule.md)
+ [unifiedRoleManagementPolicyExpirationRule](unifiedrolemanagementpolicyexpirationrule.md)
+ [unifiedRoleManagementPolicyNotificationRule](unifiedrolemanagementpolicynotificationrule.md)


Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador da regra. Herdado da [entidade](../resources/entity.md). Somente leitura.|
|destino|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)| Define detalhes do escopo direcionado pela regra de política de gerenciamento de função. Os detalhes podem incluir o tipo de entidade de segurança, o tipo de atribuição de função e as ações que afetam uma função. Suporta `$filter` (`eq`, `ne`).|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  }
}
```

