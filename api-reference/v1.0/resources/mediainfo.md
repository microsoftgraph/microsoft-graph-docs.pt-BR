---
title: tipo de recurso mediaInfo
description: As informações de mídia usadas em ações para prompts.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8e2f5a0d59f06449d122f4ca2db582afa4da9c39
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47965523"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="9cf8b-103">tipo de recurso mediaInfo</span><span class="sxs-lookup"><span data-stu-id="9cf8b-103">mediaInfo resource type</span></span>

<span data-ttu-id="9cf8b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cf8b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9cf8b-105">As informações de mídia usadas em ações para prompts.</span><span class="sxs-lookup"><span data-stu-id="9cf8b-105">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="9cf8b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9cf8b-106">Properties</span></span>
| <span data-ttu-id="9cf8b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9cf8b-107">Property</span></span>       | <span data-ttu-id="9cf8b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9cf8b-108">Type</span></span>    | <span data-ttu-id="9cf8b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cf8b-109">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="9cf8b-110">resourceId</span><span class="sxs-lookup"><span data-stu-id="9cf8b-110">resourceId</span></span>     | <span data-ttu-id="9cf8b-111">String</span><span class="sxs-lookup"><span data-stu-id="9cf8b-111">String</span></span>  | <span data-ttu-id="9cf8b-112">Opcional.</span><span class="sxs-lookup"><span data-stu-id="9cf8b-112">Optional.</span></span> <span data-ttu-id="9cf8b-113">Usada para identificar exclusivamente o recurso.</span><span class="sxs-lookup"><span data-stu-id="9cf8b-113">Used to uniquely identity the resource.</span></span> <span data-ttu-id="9cf8b-114">Se passadas, o URI de prompt será armazenado em cache em relação a este ResourceId como uma chave.</span><span class="sxs-lookup"><span data-stu-id="9cf8b-114">If passed in, the prompt uri will be cached against this resourceId as a key.</span></span> |
| <span data-ttu-id="9cf8b-115">URI</span><span class="sxs-lookup"><span data-stu-id="9cf8b-115">uri</span></span>            | <span data-ttu-id="9cf8b-116">String</span><span class="sxs-lookup"><span data-stu-id="9cf8b-116">String</span></span>  | <span data-ttu-id="9cf8b-117">Caminho para o prompt que será reproduzido.</span><span class="sxs-lookup"><span data-stu-id="9cf8b-117">Path to the prompt that will be played.</span></span> <span data-ttu-id="9cf8b-118">O atualmente oferece suporte somente a exemplos de arquivo Wave (. wav), de canal único e 16 bits com uma taxa de amostragem de 16.000 (16 kHz).</span><span class="sxs-lookup"><span data-stu-id="9cf8b-118">Currently supports only Wave file (.wav) format, single-channel, 16-bit samples with a 16,000 (16KHz) sampling rate.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="9cf8b-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9cf8b-119">JSON representation</span></span>

<span data-ttu-id="9cf8b-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9cf8b-120">The following is a JSON representation of the resource.</span></span>

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

