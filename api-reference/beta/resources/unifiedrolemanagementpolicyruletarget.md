---
title: Tipo de recurso unifiedRoleManagementPolicyRuleTarget
description: Um unifiedRoleManagementPolicyRuleTarget especifica o destino associado à política de gerenciamento de função.
author: carolinetempleton
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 6906d88c7430391fc1fcaf322c8d19ed72ab65b1
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695185"
---
# <a name="unifiedrolemanagementpolicyruletarget-resource-type"></a>Tipo de recurso unifiedRoleManagementPolicyRuleTarget

Namespace: microsoft.graph

Um unifiedRoleManagementPolicyRuleTarget especifica o destino associado à política de gerenciamento de função.


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|chamador|String|O chamador do destino da regra de política. Os valores permitidos são: `None` `Admin` , , `EndUser` .|
|enforcedSettings|Coleção de cadeias de caracteres|A lista de configurações que são impostas e não podem ser substituídos por escopos filho. Use `All` para todas as configurações.|
|inheritableSettings|Coleção de cadeias de caracteres|A lista de configurações que podem ser herdadas por escopos filho. Use `All` para todas as configurações.|
|level|String|O nível do destino da regra de política. Os valores permitidos são: `Eligibility` , `Assignment` .    |
|operations|Coleção de cadeias de caracteres|As operações para o destino da regra de política. Os valores permitidos são: `All` , , , , , , , , `Activate` `Deactivate` `Assign` `Update` `Remove` `Extend` `Renew` .|

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

