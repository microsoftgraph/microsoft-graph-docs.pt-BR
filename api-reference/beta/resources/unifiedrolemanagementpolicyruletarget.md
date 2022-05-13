---
title: Tipo de recurso unifiedRoleManagementPolicyRuleTarget
description: Um unifiedRoleManagementPolicyRuleTarget especifica o destino associado à política de gerenciamento de função.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9681efd333a4ea8db98d7a99f481c473dae3c6fb
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2022
ms.locfileid: "65399114"
---
# <a name="unifiedrolemanagementpolicyruletarget-resource-type"></a>Tipo de recurso unifiedRoleManagementPolicyRuleTarget

Namespace: microsoft.graph

Um unifiedRoleManagementPolicyRuleTarget especifica o destino associado à política de gerenciamento de função.


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Chamador|Cadeia de caracteres|O chamador do destino da regra de política. Os valores permitidos são: `None`, `Admin`, `EndUser`.|
|enforcedSettings|Coleção de cadeias de caracteres|A lista de configurações que são impostas e não podem ser substituídas por escopos filho. Use `All` para todas as configurações.|
|inheritableSettings|Coleção String|A lista de configurações que podem ser herdadas por escopos filho. Use `All` para todas as configurações.|
|Nível|Cadeia de caracteres|O nível do destino da regra de política. Os valores permitidos são: `Eligibility`, `Assignment`.    |
|operations|Coleção de cadeias de caracteres|As operações para o destino da regra de política. Os valores permitidos são: `All`, `Activate`, `Deactivate`, `Assign`, `Update`, `Remove`, `Extend`, `Renew`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|targetObjects|Coleção [directoryObject](../resources/directoryobject.md)|A coleção de usuários, grupos e servicePrincipals que estão no escopo da política. Se não for especificado, todos os objetos estão no escopo da política.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyRuleTarget",
  "caller": "String",
  "operations": [
    "String"
  ],
  "level": "String",
  "inheritableSettings": [
    "String"
  ],
  "enforcedSettings": [
    "String"
  ]
}
```

