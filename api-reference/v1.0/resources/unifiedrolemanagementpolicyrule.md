---
title: Tipo de recurso unifiedRoleManagementPolicyRule
description: Um tipo abstrato que define as regras associadas às políticas de gerenciamento de função.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 1ef9d1e4998a46f503b8960c2c0c9fca452a5c08
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2022
ms.locfileid: "65246976"
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

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador da regra. Herdado da [entidade](../resources/entity.md). Somente leitura.|
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

