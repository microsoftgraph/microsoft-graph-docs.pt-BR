---
title: Tipo de recurso unifiedRoleManagementPolicyExpirationRule
description: Um tipo derivado do tipo de recurso unifiedRoleManagementPolicyRule que define a duração máxima que uma função pode ser atribuída a uma entidade de segurança (por meio de atribuição direta ou por meio da ativação de elegibilidade)..
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2a48a9b84090b0d241e310ec4f8eada07e538d1d
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133881"
---
# <a name="unifiedrolemanagementpolicyexpirationrule-resource-type"></a>Tipo de recurso unifiedRoleManagementPolicyExpirationRule

Namespace: microsoft.graph

Um tipo derivado do tipo de recurso [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) que define a duração máxima que uma função pode ser atribuída a uma entidade de segurança (por meio de atribuição direta ou por meio da ativação de elegibilidade).

## <a name="methods"></a>Métodos

Nenhum.


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador da regra. Herdado da [entidade](../resources/entity.md).|
|isExpirationRequired|Booliano|Indica se a expiração é necessária ou se é uma atribuição ou qualificação permanentemente ativa. |
|maximumDuration|Duração| A duração máxima permitida para qualificação ou atribuição que não é permanente. Obrigatório quando **isExpirationRequired** é `true`. |
|destino|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|Define detalhes do escopo direcionado pela regra de expiração. Os detalhes podem incluir o tipo de entidade de segurança, o tipo de atribuição de função e as ações que afetam uma função. Herdado [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md). Suporta `$filter` (`eq`, `ne`).|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyExpirationRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyExpirationRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "isExpirationRequired": "Boolean",
  "maximumDuration": "String (duration)"
}
```

