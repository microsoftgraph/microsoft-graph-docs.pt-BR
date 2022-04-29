---
title: Tipo de recurso unifiedRoleManagementPolicyRule
description: Um tipo abstrato que define as regras associadas às políticas de gerenciamento de função.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 06db472f1af4634d409f51afb788dfca80d33dda
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133880"
---
# <a name="unifiedrolemanagementpolicyrule-resource-type"></a>Tipo de recurso unifiedRoleManagementPolicyRule

Namespace: microsoft.graph


Um tipo abstrato que define as regras associadas às políticas de gerenciamento de função. Esse tipo abstrato é herdado pelos seguintes recursos que definem os vários tipos de regras e suas configurações associadas às políticas de gerenciamento de função.
+ [unifiedRoleManagementPolicyApprovalRule](unifiedrolemanagementpolicyapprovalrule.md)
+ [unifiedRoleManagementPolicyAuthenticationContextRule](unifiedrolemanagementpolicyauthenticationcontextrule.md)
+ [unifiedRoleManagementPolicyEnablementRule](unifiedrolemanagementpolicyenablementrule.md)
+ [unifiedRoleManagementPolicyExpirationRule](unifiedrolemanagementpolicyexpirationrule.md)
+ [unifiedRoleManagementPolicyNotificationRule](unifiedrolemanagementpolicynotificationrule.md)


Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Methods

Nenhum.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador da regra. Herdado da [entidade](../resources/entity.md). Somente leitura.|
|destino|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)| **Não implementado.** Define detalhes do escopo direcionado pela regra de política de gerenciamento de função. Os detalhes podem incluir o tipo de entidade de segurança, o tipo de atribuição de função e as ações que afetam uma função. Suporta `$filter` (`eq`, `ne`).|

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

