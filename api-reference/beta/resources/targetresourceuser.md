---
title: tipo de recurso de targetResourceUser
description: Indica o objeto de usuário que foi adicionado, atualizado ou excluído por administradores como parte da atividade de auditoria. Derivado do recurso targetResource.
localization_priority: Normal
ms.openlocfilehash: 9c71ead1b358b72a1b531abac56018fa71d084e8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831924"
---
# <a name="targetresourceuser-resource-type"></a>tipo de recurso de targetResourceUser
Indica o objeto de usuário que foi adicionado, atualizado ou excluído por administradores como parte da atividade de auditoria. Derivado do recurso [targetResource](targetresource.md) .


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|userPrincipalName|Cadeia de caracteres|Indica a Id exclusiva do usuário. Se refere à Id de usuário para um usuário específico.|

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
