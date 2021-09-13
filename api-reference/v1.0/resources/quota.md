---
author: JeremyKelley
ms.date: 09/10/2017
title: Cota
ms.localizationpriority: medium
description: O recurso quota fornece detalhes sobre restrições de espaço em um recurso Drive.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 71f0f29c4ab6979f7154940e9007665d020b7f68
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59143807"
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
| total         | Int64  | Espaço de armazenamento permitido total, em bytes. Somente leitura.                           |
| used          | Int64  | Espaço total, em bytes. Somente leitura.                                      |
| remaining     | Int64  | Espaço total restante antes de atingir o limite de cota, em bytes. Somente leitura. |
| deleted       | Int64  | Espaço total consumido por arquivos na Lixeira, em bytes. Somente leitura.      |
| estado         | string | Valor de enumeração que indica o estado do espaço de armazenamento. Somente leitura. |
| storagePlanInformation  | [storagePlanInformation](storageplaninformation.md) | Informações sobre os planos de cota de armazenamento da unidade. Somente em Pessoal OneDrive.|

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

