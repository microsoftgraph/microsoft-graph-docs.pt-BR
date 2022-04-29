---
title: Tipo de recurso unifiedRoleManagementPolicyEnablementRule
description: Um tipo derivado do tipo de recurso unifiedRoleManagementPolicyRule que define as regras para habilitar a atribuição, por exemplo, habilitar a MFA, justificativa sobre atribuições ou informações de tíquete.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d9a964a31180348c4e2f797f7ce4769965f17708
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133847"
---
# <a name="unifiedrolemanagementpolicyenablementrule-resource-type"></a>Tipo de recurso unifiedRoleManagementPolicyEnablementRule

Namespace: microsoft.graph

Um tipo derivado do tipo de recurso [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) que define as regras para habilitar a atribuição, por exemplo, habilitar a MFA, justificativa sobre atribuições ou informações de tíquete.

## <a name="methods"></a>Métodos

Nenhum.


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|enabledRules|Coleção de cadeias de caracteres|A coleção de regras que estão habilitadas para essa regra de política. Por exemplo, `MultiFactorAuthentication`, `Ticketing`e `Justification`.|
|id|Cadeia de caracteres|Identificador da regra. Herdado da [entidade](../resources/entity.md).|
|destino|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|Define detalhes do escopo direcionado pela regra de habilitação. Os detalhes podem incluir o tipo de entidade de segurança, o tipo de atribuição de função e as ações que afetam uma função. Herdado [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md). Suporta `$filter` (`eq`, `ne`).|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyEnablementRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyEnablementRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "enabledRules": [
    "String"
  ]
}
```

