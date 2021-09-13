---
title: Tipo de recurso unifiedRoleManagementPolicyRule
description: Um unifiedRoleManagementPolicyRule especifica a regra associada a uma política de gerenciamento de função. É abstrato.
author: shauliu1
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b2d75b5ced7ca80bbbf9de4cb0feee2456e3eada
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59056988"
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

