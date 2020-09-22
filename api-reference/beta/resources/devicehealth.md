---
title: tipo de recurso deviceHealth
description: Representa a integridade de um dispositivo, incluindo quaisquer erros.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 7da256308ee63607d7d2d0e7ba62cb3030db4835
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049853"
---
# <a name="devicehealth-resource-type"></a><span data-ttu-id="d36fd-103">tipo de recurso deviceHealth</span><span class="sxs-lookup"><span data-stu-id="d36fd-103">deviceHealth resource type</span></span>

<span data-ttu-id="d36fd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d36fd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d36fd-105">Representa a integridade de um dispositivo, incluindo quaisquer erros.</span><span class="sxs-lookup"><span data-stu-id="d36fd-105">Represents a device's health, including any errors.</span></span>

## <a name="properties"></a><span data-ttu-id="d36fd-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d36fd-106">Properties</span></span>
| <span data-ttu-id="d36fd-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d36fd-107">Property</span></span>     | <span data-ttu-id="d36fd-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d36fd-108">Type</span></span>        | <span data-ttu-id="d36fd-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d36fd-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d36fd-110">lastConnectionTime</span><span class="sxs-lookup"><span data-stu-id="d36fd-110">lastConnectionTime</span></span>|<span data-ttu-id="d36fd-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d36fd-111">DateTimeOffset</span></span>|<span data-ttu-id="d36fd-112">A última vez que o dispositivo foi conectado.</span><span class="sxs-lookup"><span data-stu-id="d36fd-112">The last time the device was connected.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d36fd-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d36fd-113">JSON representation</span></span>

<span data-ttu-id="d36fd-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d36fd-114">The following is a JSON representation of the resource.</span></span>

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

