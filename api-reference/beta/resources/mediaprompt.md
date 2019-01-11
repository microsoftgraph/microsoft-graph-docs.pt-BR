---
title: tipo de recurso de mediaPrompt
description: O tipo de mediaPrompt.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 31e1e0e1d842c758cddfb78a39b2dcc185e97ec9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884263"
---
# <a name="mediaprompt-resource-type"></a><span data-ttu-id="33b35-103">tipo de recurso de mediaPrompt</span><span class="sxs-lookup"><span data-stu-id="33b35-103">mediaPrompt resource type</span></span>

> <span data-ttu-id="33b35-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="33b35-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33b35-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="33b35-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="33b35-106">O tipo de mediaPrompt.</span><span class="sxs-lookup"><span data-stu-id="33b35-106">The mediaPrompt type.</span></span>

## <a name="properties"></a><span data-ttu-id="33b35-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="33b35-107">Properties</span></span>

| <span data-ttu-id="33b35-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33b35-108">Property</span></span>    | <span data-ttu-id="33b35-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="33b35-109">Type</span></span>                      | <span data-ttu-id="33b35-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="33b35-110">Description</span></span>                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| <span data-ttu-id="33b35-111">loop</span><span class="sxs-lookup"><span data-stu-id="33b35-111">loop</span></span>        | <span data-ttu-id="33b35-112">Int32</span><span class="sxs-lookup"><span data-stu-id="33b35-112">Int32</span></span>                     | <span data-ttu-id="33b35-113">A contagem de loop.</span><span class="sxs-lookup"><span data-stu-id="33b35-113">The loop count.</span></span> <span data-ttu-id="33b35-114">o valor 0 indica para executar um loop indefinidamente.</span><span class="sxs-lookup"><span data-stu-id="33b35-114">0 value indicates to loop infinitely.</span></span> <span data-ttu-id="33b35-115">O valor padrão é `1`.</span><span class="sxs-lookup"><span data-stu-id="33b35-115">The default value is `1`.</span></span> |
| <span data-ttu-id="33b35-116">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="33b35-116">mediaInfo</span></span>   | [<span data-ttu-id="33b35-117">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="33b35-117">mediaInfo</span></span>](mediainfo.md) | <span data-ttu-id="33b35-118">As informações de mídia</span><span class="sxs-lookup"><span data-stu-id="33b35-118">The media information</span></span>                                                           |

## <a name="json-representation"></a><span data-ttu-id="33b35-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="33b35-119">JSON representation</span></span>

<span data-ttu-id="33b35-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="33b35-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->

```json
{
  "loop": 1024,
  "mediaInfo": { "@odata.type": "#microsoft.graph.mediaInfo" }
}
```

## <a name="example"></a><span data-ttu-id="33b35-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33b35-121">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->
```json
{
  "mediaInfo": {
    "uri": "https://cdn.contoso.com/beep.wav",
    "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
  },
  "loop": 5
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mediaPrompt resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
