---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Compartilhados
ms.openlocfilehash: 1d828310a226edd0443ff3b5f60156df1e7c98cb
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="shared-resource-type"></a>Tipo de recurso compartilhado

O recurso **Shared** indica que um DriveItem foi compartilhado com outras pessoas.
O recurso inclui informações sobre como o item é compartilhado.

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
| scope          | String                        | Indica o escopo de como o item é compartilhado: `anonymous`, `organization` ou `users`. Somente leitura.
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

<!-- {
  "type": "#page.annotation",
  "description": "The shared facet provides info about shared items.",
  "keywords": "shared,share,item,facet,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Shared"
} -->
