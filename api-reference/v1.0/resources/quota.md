---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Cota
localization_priority: Normal
description: O recurso quota fornece detalhes sobre restrições de espaço em um recurso Drive.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 293daf950beb5cdf3cbd791a1e8bf0d4b92a220b
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44864207"
---
# <a name="quota-resource-type"></a>Tipo de recurso Quota

Namespace: microsoft.graph

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
  "storagePlanInformation": {
    "upgradeAvailable": true
  },
  "total": 1024,
  "used": 1024
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade | Tipo   | Descrição                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| total         | Int64  | Total allowed storage space, in bytes. Read-only.                           |
| used          | Int64  | Total space used, in bytes. Read-only.                                      |
| remaining     | Int64  | Total space remaining before reaching the quota limit, in bytes. Read-only. |
| deleted       | Int64  | Total space consumed by files in the recycle bin, in bytes. Read-only.      |
| estado         | string | Enumeration value that indicates the state of the storage space. Read-only. |
| Adicionadostorageplaninformation  | [Adicionadostorageplaninformation](storageplaninformation.md) | Informações sobre os planos de cota de armazenamento da unidade. Somente no OneDrive pessoal.|

## <a name="state-enumeration"></a>Enumeração de Estado

| Valor      | Descrição                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | A unidade tem bastante cota restante.                                                                                                                               |
| `nearing`  | A cota restante é inferior a 10% do espaço de cota total.                                                                                                                      |
| `critical` | A cota restante é inferior a 1% do espaço de cota total.                                                                                                                       |
| `exceeded` | The used quota has exceeded the total quota. New files or folders cannot be added to the drive until it is under the total quota amount or more storage space is purchased. |

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
