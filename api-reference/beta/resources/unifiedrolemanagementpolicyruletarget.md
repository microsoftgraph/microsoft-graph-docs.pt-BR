---
title: Tipo de recurso unifiedRoleManagementPolicyRuleTarget
description: Um unifiedRoleManagementPolicyRuleTarget especifica o destino associado à política de gerenciamento de função.
author: shauliu1
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c4d7bfb6744c3272e9237590b4d17c5e1d79b0f9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59074441"
---
# <a name="unifiedrolemanagementpolicyruletarget-resource-type"></a>Tipo de recurso unifiedRoleManagementPolicyRuleTarget

Namespace: microsoft.graph

Um unifiedRoleManagementPolicyRuleTarget especifica o destino associado à política de gerenciamento de função.


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|chamador|String|O chamador do destino da regra de política. Os valores permitidos são: `None` `Admin` , , `EndUser` .|
|enforcedSettings|Conjunto de cadeias de caracteres|A lista de configurações que são impostas e não podem ser substituídos por escopos filho. Use `All` para todas as configurações.|
|inheritableSettings|Conjunto de cadeias de caracteres|A lista de configurações que podem ser herdadas por escopos filho. Use `All` para todas as configurações.|
|level|String|O nível do destino da regra de política. Os valores permitidos são: `Eligibility` , `Assignment` .    |
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

