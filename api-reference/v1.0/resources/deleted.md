---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Deleted
localization_priority: Normal
description: O recurso Deleted indica que o item foi excluído.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c81c2623d49d40f1a4619c7f964ba9b7f0b94cf2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531682"
---
# <a name="deleted-facet"></a>Faceta Deleted

Namespace: microsoft.graph

O recurso **Deleted** indica que o item foi excluído. Nesta versão da API, a presença (não nulo) do valor do recurso indica que o arquivo foi excluído. Um valor nulo (ou faltante) indica que o arquivo não foi excluído.

Consulte [exibir alterações de um item](../api/driveitem-delta.md) para saber mais sobre como acompanhar as alterações e localizar itens excluídos.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  "state"
  ],
  "@odata.type": "microsoft.graph.deleted"
}-->
```json
{
  "state": "string"
}
```
## <a name="properties"></a>Propriedades

| Propriedade | Tipo   | Descrição                               |
|:---------|:-------|:------------------------------------------|
| state    | String | Representa o estado do item excluído. |

## <a name="remarks"></a>Comentários 

Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted"
} -->
