---
title: Tipo de recurso unifiedRoleManagementPolicyRuleTarget
description: Um unifiedRoleManagementPolicyRuleTarget especifica o destino associado à política de gerenciamento de função.
author: japere
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3d51be1fe5cd4f16f443bf095de4f276dad5d5b8
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2022
ms.locfileid: "64508472"
---
# <a name="unifiedrolemanagementpolicyruletarget-resource-type"></a>Tipo de recurso unifiedRoleManagementPolicyRuleTarget

Namespace: microsoft.graph

Um unifiedRoleManagementPolicyRuleTarget especifica o destino associado à política de gerenciamento de função.


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|chamador|Cadeia de caracteres|O chamador do destino da regra de política. Os valores permitidos são: `None`, `Admin`, . `EndUser`|
|enforcedSettings|Coleção de cadeias de caracteres|A lista de configurações que são impostas e não podem ser substituídos por escopos filho. Use `All` para todas as configurações.|
|inheritableSettings|Coleção String|A lista de configurações que podem ser herdadas por escopos filho. Use `All` para todas as configurações.|
|level|Cadeia de caracteres|O nível do destino da regra de política. Os valores permitidos são: `Eligibility`, `Assignment`.    |
|operations|Coleção de cadeias de caracteres|As operações para o destino da regra de política. Os valores permitidos são: , , , , , `Update`, `Remove`, `Extend`, `Renew`. `Assign``Deactivate``Activate``All`|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|targetObjects|Conjunto [directoryObject](../resources/directoryobject.md)|A coleção de usuários, grupos e servicePrincipals que estão no escopo da política. Se não for especificado, todos os objetos estão no escopo da política.|

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

