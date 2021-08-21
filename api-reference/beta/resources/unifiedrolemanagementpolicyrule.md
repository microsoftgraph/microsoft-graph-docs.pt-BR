---
title: Tipo de recurso unifiedRoleManagementPolicyRule
description: Um unifiedRoleManagementPolicyRule especifica a regra associada a uma política de gerenciamento de função. É abstrato.
author: shauliu1
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 99dc73128cbaadce2bbd61d8f704ce20e2a60d69
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453874"
---
# <a name="unifiedrolemanagementpolicyrule-resource-type"></a>Tipo de recurso unifiedRoleManagementPolicyRule

Namespace: microsoft.graph

Um unifiedRoleManagementPolicyRule especifica a regra associada a uma política de gerenciamento de função. É abstrato.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedRoleManagementPolicyRules](../api/unifiedrolemanagementpolicyrule-list.md)|[Coleção unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Obter uma lista dos [objetos unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) e suas propriedades.|
|[Obter unifiedRoleManagementPolicyRule](../api/unifiedrolemanagementpolicyrule-get.md)|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Leia as propriedades e as relações de [um objeto unifiedRoleManagementPolicyRule.](../resources/unifiedrolemanagementpolicyrule.md)|
|[Atualizar unifiedRoleManagementPolicyRule](../api/unifiedrolemanagementpolicyrule-update.md)|[unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)|Atualize as propriedades de [um objeto unifiedRoleManagementPolicyRule.](../resources/unifiedrolemanagementpolicyrule.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo da regra.|
|destino|[unifiedRoleManagementPolicyRuleTarget](../resources/unifiedrolemanagementpolicyruletarget.md)|O destino da regra de política.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRule",
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

