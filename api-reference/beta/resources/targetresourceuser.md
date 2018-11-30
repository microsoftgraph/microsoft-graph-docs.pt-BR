---
title: tipo de recurso de targetResourceUser
description: Indica o objeto de usuário que foi adicionado, atualizado ou excluído por administradores como parte da atividade de auditoria. Derivado do recurso targetResource.
ms.openlocfilehash: 632d0551b3aba434c3309c8c874947708eb9a9f5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036427"
---
# <a name="targetresourceuser-resource-type"></a>tipo de recurso de targetResourceUser
Indica o objeto de usuário que foi adicionado, atualizado ou excluído por administradores como parte da atividade de auditoria. Derivado do recurso [targetResource](targetresource.md) .


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|userPrincipalName|String|Indica a Id exclusiva do usuário. Se refere à Id de usuário para um usuário específico.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourceUser"
}-->

```json
{
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourceUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->