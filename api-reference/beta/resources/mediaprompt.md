---
title: tipo de recurso mediaPrompt
description: O tipo mediaPrompt.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cd2a700298c6f8163e3162e244f66468e1a94e7c
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932482"
---
# <a name="mediaprompt-resource-type"></a><span data-ttu-id="06257-103">tipo de recurso mediaPrompt</span><span class="sxs-lookup"><span data-stu-id="06257-103">mediaPrompt resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06257-104">O tipo mediaPrompt.</span><span class="sxs-lookup"><span data-stu-id="06257-104">The mediaPrompt type.</span></span>

## <a name="properties"></a><span data-ttu-id="06257-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="06257-105">Properties</span></span>

| <span data-ttu-id="06257-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06257-106">Property</span></span>    | <span data-ttu-id="06257-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="06257-107">Type</span></span>                      | <span data-ttu-id="06257-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="06257-108">Description</span></span>                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| <span data-ttu-id="06257-109">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="06257-109">mediaInfo</span></span>   | [<span data-ttu-id="06257-110">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="06257-110">mediaInfo</span></span>](mediainfo.md) | <span data-ttu-id="06257-111">As informações de mídia</span><span class="sxs-lookup"><span data-stu-id="06257-111">The media information</span></span>                                                           |

## <a name="json-representation"></a><span data-ttu-id="06257-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="06257-112">JSON representation</span></span>

<span data-ttu-id="06257-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="06257-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->

```json
{
  "mediaInfo": { "@odata.type": "#microsoft.graph.mediaInfo" }
}
```

## <a name="example"></a><span data-ttu-id="06257-114">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06257-114">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->
```json
{
  "@odata.type": "#microsoft.graph.mediaPrompt",
  "mediaInfo": {
    "@odata.type": "#microsoft.graph.mediaInfo",
    "uri": "https://cdn.contoso.com/beep.wav",
    "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaPrompt resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
