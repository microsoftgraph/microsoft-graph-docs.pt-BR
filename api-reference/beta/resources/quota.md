---
author: JeremyKelley
description: O recurso de cota fornece detalhes sobre restrições de espaço em um recurso de unidade.
ms.date: 09/10/2017
title: Cota
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: fb27c29c70c0775ad59bf23c33348aaf490ebaed
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176731"
---
# <a name="quota-resource-type"></a>tipo de recurso de cota

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O **recurso** de cota fornece detalhes sobre restrições de espaço em um recurso [de](drive.md) unidade.

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

| Propriedade               | Tipo                                                | Descrição                                                                   |
| :--------------------- | :-------------------------------------------------- | :---------------------------------------------------------------------------- |
| total                  | Int64                                               | Espaço de armazenamento permitido total, em bytes. Somente leitura.                             |
| used                   | Int64                                               | Espaço total, em bytes. Somente leitura.                                        |
| remaining              | Int64                                               | Espaço total restante antes de atingir o limite de cota, em bytes. Somente leitura.   |
| deleted                | Int64                                               | Espaço total consumido por arquivos na Lixeira, em bytes. Somente leitura.        |
| estado                  | string                                              | Valor de enumeração que indica o estado do espaço de armazenamento. Somente leitura.   |
| storagePlanInformation | [storagePlanInformation](storageplaninformation.md) | Informações sobre os planos de cota de armazenamento da unidade. Somente em Pessoal OneDrive. |

### <a name="state-enumeration-values"></a>Valores de enumeração de estado

| Valor      | Descrição                                                                                                                                                                 |
| :--------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `normal`   | A unidade tem bastante cota restante.                                                                                                                               |
| `nearing`  | A cota restante é inferior a 10% do espaço de cota total.                                                                                                                      |
| `critical` | A cota restante é inferior a 1% do espaço de cota total.                                                                                                                       |
| `exceeded` | A cota usada excedeu a cota total. Novos arquivos ou pastas não podem ser adicionadas à unidade até que ela esteja abaixo da quantidade total de cotas ou mais espaço de armazenamento seja adquirido. |

<!--
{
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/Quota",
  "suppressions": []
}
-->
