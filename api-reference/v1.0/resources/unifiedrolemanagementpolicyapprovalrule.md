---
title: Tipo de recurso unifiedRoleManagementPolicyApprovalRule
description: Um tipo derivado do tipo de recurso unifiedRoleManagementPolicyRule que define regras para aprovar uma atribuição de função.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: cc3e0033a7dfc51afe921a55046178a04a453f6b
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133843"
---
# <a name="unifiedrolemanagementpolicyapprovalrule-resource-type"></a>Tipo de recurso unifiedRoleManagementPolicyApprovalRule

Namespace: microsoft.graph

Um tipo derivado do tipo de recurso [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) que define regras para aprovar uma atribuição de função.

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador da regra. Herdado da [entidade](../resources/entity.md).|
|configuração|[approvalSettings](../resources/approvalsettings.md)|As configurações para aprovação da atribuição de função.|
|destino|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|Define detalhes do escopo direcionado pela regra de aprovação. Os detalhes podem incluir o tipo de entidade de segurança, o tipo de atribuição de função e as ações que afetam uma função. Herdado [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md). Suporta `$filter` (`eq`, `ne`).|

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

