---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Cota
localization_priority: Normal
description: O recurso quota fornece detalhes sobre restrições de espaço em um recurso Drive.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ee93ddfe54e785ea8a8fa245ab3828c548928cc0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034955"
---
# <a name="quota-resource-type"></a>Tipo de recurso Quota

O recurso **quota** fornece detalhes sobre restrições de espaço em um recurso [Drive](drive.md).

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.quota"
}-->

```json
{
  "deleted": 1024,
  "remaining": 1024,
  "state": "normal | nearing | critical | exceeded",
  "total": 1024,
  "used": 1024
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade | Tipo   | Descrição                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| total         | Int64  | Espaço de armazenamento permitido total, em bytes. Somente leitura.                           |
| used          | Int64  | Espaço total, em bytes. Somente leitura.                                      |
| remaining     | Int64  | Espaço total restante antes de atingir o limite de cota, em bytes. Somente leitura. |
| deleted       | Int64  | Espaço total consumido por arquivos na Lixeira, em bytes. Somente leitura.      |
| estado         | string | Valor de enumeração que indica o estado do espaço de armazenamento. Somente leitura. |

## <a name="state-enumeration"></a>Enumeração de Estado

| Valor      | Descrição                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | A unidade tem bastante cota restante.                                                                                                                               |
| `nearing`  | A cota restante é inferior a 10% do espaço de cota total.                                                                                                                      |
| `critical` | A cota restante é inferior a 1% do espaço de cota total.                                                                                                                       |
| `exceeded` | A cota usada excedeu a cota total. Novos arquivos ou pastas não podem ser adicionadas à unidade até que ela esteja abaixo da quantidade total de cotas ou mais espaço de armazenamento seja adquirido. |

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/quota.md:
      Found potential enums in resource example that weren't defined in a table:(normal, nearing,critical,exceeded) are in resource, but () are in table"
  ],
  "tocPath": "Facets/Quota"
} -->
