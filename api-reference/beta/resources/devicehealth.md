---
title: tipo de recurso deviceHealth
description: Representa a integridade de um dispositivo, incluindo quaisquer erros.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: efd8b1e7722eabcacd05512b0101735d677d9b89
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895516"
---
# <a name="devicehealth-resource-type"></a><span data-ttu-id="c91db-103">tipo de recurso deviceHealth</span><span class="sxs-lookup"><span data-stu-id="c91db-103">deviceHealth resource type</span></span>

<span data-ttu-id="c91db-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c91db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c91db-105">Representa a integridade de um dispositivo, incluindo quaisquer erros.</span><span class="sxs-lookup"><span data-stu-id="c91db-105">Represents a device's health, including any errors.</span></span>

## <a name="properties"></a><span data-ttu-id="c91db-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c91db-106">Properties</span></span>
| <span data-ttu-id="c91db-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c91db-107">Property</span></span>     | <span data-ttu-id="c91db-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c91db-108">Type</span></span>        | <span data-ttu-id="c91db-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c91db-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c91db-110">lastConnectionTime</span><span class="sxs-lookup"><span data-stu-id="c91db-110">lastConnectionTime</span></span>|<span data-ttu-id="c91db-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c91db-111">DateTimeOffset</span></span>|<span data-ttu-id="c91db-112">A última vez que o dispositivo foi conectado.</span><span class="sxs-lookup"><span data-stu-id="c91db-112">The last time the device was connected.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c91db-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c91db-113">JSON representation</span></span>

<span data-ttu-id="c91db-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c91db-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.deviceHealth"
}-->

```json
{
    "lastConnectionTime": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceHealth resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->