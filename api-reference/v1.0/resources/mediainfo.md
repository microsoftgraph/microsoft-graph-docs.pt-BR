---
title: tipo de recurso mediaInfo
description: As informações de mídia usadas em ações para prompts.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9d9b8f4709d3379afda8e30fec2b7db64a474a0e
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865657"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="80ba7-103">tipo de recurso mediaInfo</span><span class="sxs-lookup"><span data-stu-id="80ba7-103">mediaInfo resource type</span></span>

<span data-ttu-id="80ba7-104">As informações de mídia usadas em ações para prompts.</span><span class="sxs-lookup"><span data-stu-id="80ba7-104">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="80ba7-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="80ba7-105">Properties</span></span>
| <span data-ttu-id="80ba7-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80ba7-106">Property</span></span>       | <span data-ttu-id="80ba7-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="80ba7-107">Type</span></span>    | <span data-ttu-id="80ba7-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="80ba7-108">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="80ba7-109">resourceId</span><span class="sxs-lookup"><span data-stu-id="80ba7-109">resourceId</span></span>     | <span data-ttu-id="80ba7-110">String</span><span class="sxs-lookup"><span data-stu-id="80ba7-110">String</span></span>  | <span data-ttu-id="80ba7-111">Opcional.</span><span class="sxs-lookup"><span data-stu-id="80ba7-111">Optional.</span></span> <span data-ttu-id="80ba7-112">Usada para identificar exclusivamente o recurso.</span><span class="sxs-lookup"><span data-stu-id="80ba7-112">Used to uniquely identity the resource.</span></span> <span data-ttu-id="80ba7-113">Se passadas, o URI de prompt será armazenado em cache em relação a este ResourceId como uma chave.</span><span class="sxs-lookup"><span data-stu-id="80ba7-113">If passed in, the prompt uri will be cached against this resourceId as a key.</span></span> |
| <span data-ttu-id="80ba7-114">URI</span><span class="sxs-lookup"><span data-stu-id="80ba7-114">uri</span></span>            | <span data-ttu-id="80ba7-115">String</span><span class="sxs-lookup"><span data-stu-id="80ba7-115">String</span></span>  | <span data-ttu-id="80ba7-116">Caminho para o prompt que será reproduzido.</span><span class="sxs-lookup"><span data-stu-id="80ba7-116">Path to the prompt that will be played.</span></span> <span data-ttu-id="80ba7-117">O atualmente oferece suporte somente a exemplos de arquivo Wave (. wav), de canal único e 16 bits com uma taxa de amostragem de 16.000 (16 kHz).</span><span class="sxs-lookup"><span data-stu-id="80ba7-117">Currently supports only Wave file (.wav) format, single-channel, 16-bit samples with a 16,000 (16KHz) sampling rate.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="80ba7-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="80ba7-118">JSON representation</span></span>

<span data-ttu-id="80ba7-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="80ba7-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaInfo"
}-->
```json
{
  "resourceId": "String",
  "uri": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
