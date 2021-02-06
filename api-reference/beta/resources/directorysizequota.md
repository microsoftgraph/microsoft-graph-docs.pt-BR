---
title: Tipo de recurso directorySizeQuota
description: Representa a cota de diretório total e usada de uma empresa.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: davidmu1
ms.openlocfilehash: 3af82a957e152f0edf4d87e6fdf9a7888d4b64e4
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133984"
---
# <a name="directorysizequota-resource-type"></a>Tipo de recurso directorySizeQuota

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a cota de diretório total e usada de uma empresa.

## <a name="properties"></a>Propriedades
| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|usado|Int32| Quantidade usada da cota de diretório. |
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
