---
title: Compartilhados
author: JeremyKelley
description: O recurso Shared indica que um DriveItem foi compartilhado com outras pessoas.
ms.date: 09/10/2017
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: f814ce4d6f395784c987da997e7a8b6f3f201b17
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66731909"
---
# <a name="shared-resource-type"></a>Tipo de recurso Shared

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **Shared** indica que um DriveItem foi compartilhado com outras pessoas. O recurso inclui informações sobre como o item é compartilhado.

Se um [**Driveitem**](driveitem.md) tem uma faceta **shared** não nula, o item foi compartilhada.

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.shared",
  "optionalProperties": [ "sharedBy", "sharedDateTime" ]
}-->

```json
{
  "owner": { "@odata.type": "microsoft.graph.identitySet" },
  "scope": "anonymous | organization | users",
  "sharedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "sharedDateTime": "datetime"
}
```

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo                          | Descrição
| :------------- |:------------------------------|:----------------------------
| owner          | [IdentitySet](identityset.md) | A identidade do proprietário do item compartilhado. Somente leitura.
| escopo          | String                        | Indica o escopo de como o item é compartilhado: `anonymous`, `organization` ou `users`. Somente leitura.
| sharedBy       | [identitySet](identityset.md) | A identidade do usuário que compartilhou o item. Somente leitura.
| sharedDateTime | DateTimeOffset                | A data e a hora UTC que o item foi compartilhado. Somente leitura.

## <a name="scope-values"></a>Valores de escopo

| Valor          | Descrição                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | O item é compartilhado usando-se um link que funciona para qualquer pessoa que tem o link.               |
| `organization` | O item é compartilhado usando-se um link que funciona para qualquer pessoa na organização do proprietário. |
| `users`        | O item é compartilhado apenas com usuários específicos.                                          |

## <a name="remarks"></a>Comentários

Para saber mais sobre as facetas de um **driveItem**, confira [**driveItem**](driveitem.md).

<!--
{
  "type": "#page.annotation",
  "description": "The shared facet provides info about shared items.",
  "keywords": "shared,share,item,facet,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Shared",
  "suppressions": []
}
-->


