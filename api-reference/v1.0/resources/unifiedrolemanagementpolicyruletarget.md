---
title: Tipo de recurso unifiedRoleManagementPolicyRuleTarget
description: Define detalhes do escopo direcionado pela regra de política de gerenciamento de função. Os detalhes podem incluir o tipo de entidade de segurança, o tipo de atribuição de função e as ações que afetam uma função.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 1ae571305de5d7f20635467e65d38090761b21ce
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133879"
---
# <a name="unifiedrolemanagementpolicyruletarget-resource-type"></a>Tipo de recurso unifiedRoleManagementPolicyRuleTarget

Namespace: microsoft.graph

Define detalhes do escopo direcionado pela regra de política de gerenciamento de função. Os detalhes podem incluir o tipo de entidade de segurança, o tipo de atribuição de função e as ações que afetam uma função.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Chamador|Cadeia de caracteres|O tipo de chamador que é o destino da regra de política. Os valores permitidos são: `None`, `Admin`, `EndUser`.|
|enforcedSettings|Coleção de cadeias de caracteres|A lista de configurações de função que são impostas e não podem ser substituídas por escopos filho. Use `All` para todas as configurações.|
|inheritableSettings|Coleção de cadeias de caracteres|A lista de configurações de função que podem ser herdadas por escopos filho. Use `All` para todas as configurações.|
|Nível|Cadeia de caracteres|O tipo de atribuição de função que é o destino da regra de política. Os valores permitidos são: `Eligibility`, `Assignment`.   |
|operations|Coleção de cadeias de caracteres|As operações de gerenciamento de função que são o destino da regra de política. Os valores permitidos são: `All`, `Activate`, `Deactivate`, `Assign`, `Update`, `Remove`, `Extend`, `Renew`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|targetObjects|Coleção [directoryObject](../resources/directoryobject.md)| A coleção de usuários, grupos e entidades de serviço que estão no escopo da política. Se não for especificado, todos os objetos estão no escopo da política.|

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

