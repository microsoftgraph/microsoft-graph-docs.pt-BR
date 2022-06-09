---
author: JeremyKelley
ms.date: 09/10/2017
title: Deleted
ms.localizationpriority: medium
description: O recurso Deleted indica que o item foi excluído.
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 3ba5423b677455735323ea96738f56a7946ac200
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971263"
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
| estado    | Cadeia de caracteres | Representa o estado do item excluído. |

## <a name="remarks"></a>Comentários 

Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted"
} -->

