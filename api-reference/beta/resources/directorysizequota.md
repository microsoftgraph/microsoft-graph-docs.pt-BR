---
title: Tipo de recurso directorySizeQuota
description: Representa a cota de diretório total e usada de uma empresa.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: directory-management
author: Jumaodhiss
ms.openlocfilehash: ac8b26fababe53458b8dd3a92624d9ce0a11514a
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/19/2021
ms.locfileid: "60483012"
---
# <a name="directorysizequota-resource-type"></a>Tipo de recurso directorySizeQuota

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a cota de diretório total e usada de uma empresa.

## <a name="properties"></a>Propriedades
| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|usado|Int32| Quantidade usada da cota de diretório. |
|total|Int32| Quantidade total da cota de diretório.|

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
  "used": "Int32",
  "total": "Int32"
}
```
