---
title: tipo de recurso directorySizeQuota
description: Representa a cota de diretório total usada e de uma empresa.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 8f5f172cb8f090b71b7e0fd3c89151668c167afd
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48315595"
---
# <a name="directorysizequota-resource-type"></a>tipo de recurso directorySizeQuota

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a cota de diretório total usada e de uma empresa.

## <a name="properties"></a>Propriedades
| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|usado|Int32| Valor usado da cota de diretório. |
|total|Int32| Valor total da cota de diretório.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySizeQuota"
}-->

```json
{
  "used": 123,
  "total": 1234
}
```
