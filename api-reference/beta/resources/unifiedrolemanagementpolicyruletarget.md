---
title: Tipo de recurso unifiedRoleManagementPolicyRuleTarget
description: Um unifiedRoleManagementPolicyRuleTarget especifica o destino associado à política de gerenciamento de função.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b8b474102e0605fda38db7b0ef39b1105097ba8d5d4b7f376ec3db83e1c07541
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54145093"
---
# <a name="unifiedrolemanagementpolicyruletarget-resource-type"></a>Tipo de recurso unifiedRoleManagementPolicyRuleTarget

Namespace: microsoft.graph

Um unifiedRoleManagementPolicyRuleTarget especifica o destino associado à política de gerenciamento de função.


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|chamador|Cadeia de caracteres|O chamador do destino da regra de política. Os valores permitidos são: `None` `Admin` , , `EndUser` .|
|enforcedSettings|String collection|A lista de configurações que são impostas e não podem ser substituídos por escopos filho. Use `All` para todas as configurações.|
|inheritableSettings|String collection|A lista de configurações que podem ser herdadas por escopos filho. Use `All` para todas as configurações.|
|level|Cadeia de caracteres|O nível do destino da regra de política. Os valores permitidos são: `Eligibility` , `Assignment` .    |
|operations|String collection|As operações para o destino da regra de política. Os valores permitidos são: `All` , , , , , , , , `Activate` `Deactivate` `Assign` `Update` `Remove` `Extend` `Renew` .|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|targetObjects|Coleção [directoryObject](../resources/directoryobject.md)|A coleção de usuários, grupos e servicePrincipals que estão no escopo da política. Se não for especificado, todos os objetos estão no escopo da política.|
-->
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

