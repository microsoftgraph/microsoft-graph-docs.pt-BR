---
title: tipo de recurso mediaInfo
description: As informações de mídia usadas em ações para prompts.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d17117880cf736870d2728a9666af689a4296d04
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913293"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="e8b6f-103">tipo de recurso mediaInfo</span><span class="sxs-lookup"><span data-stu-id="e8b6f-103">mediaInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8b6f-104">As informações de mídia usadas em ações para prompts.</span><span class="sxs-lookup"><span data-stu-id="e8b6f-104">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="e8b6f-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e8b6f-105">Properties</span></span>
| <span data-ttu-id="e8b6f-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8b6f-106">Property</span></span>       | <span data-ttu-id="e8b6f-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8b6f-107">Type</span></span>    | <span data-ttu-id="e8b6f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8b6f-108">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="e8b6f-109">resourceId</span><span class="sxs-lookup"><span data-stu-id="e8b6f-109">resourceId</span></span>     | <span data-ttu-id="e8b6f-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8b6f-110">String</span></span>  | <span data-ttu-id="e8b6f-111">Opcional, usada para identificar exclusivamente o recurso.</span><span class="sxs-lookup"><span data-stu-id="e8b6f-111">Optional, used to uniquely identity the resource.</span></span> <span data-ttu-id="e8b6f-112">Se for passado, a URI do prompt será armazenada em cache para esta ResourceId como chave.</span><span class="sxs-lookup"><span data-stu-id="e8b6f-112">If passed the prompt uri will be cached against this resourceId as key.</span></span> |
| <span data-ttu-id="e8b6f-113">URI</span><span class="sxs-lookup"><span data-stu-id="e8b6f-113">uri</span></span>            | <span data-ttu-id="e8b6f-114">String</span><span class="sxs-lookup"><span data-stu-id="e8b6f-114">String</span></span>  | <span data-ttu-id="e8b6f-115">Caminho para o prompt a ser reproduzido.</span><span class="sxs-lookup"><span data-stu-id="e8b6f-115">Path to the prompt to be played.</span></span> <span data-ttu-id="e8b6f-116">Atualmente, somente os exemplos de arquivo Wave (. wav), de canal único e 16 bits com uma taxa de amostragem de 16.000 (16 kHz) só têm suporte.</span><span class="sxs-lookup"><span data-stu-id="e8b6f-116">Currently only Wave file (.wav) format, single-channel, 16-bit samples with a 16,000 (16KHz) sampling rate is only supported.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="e8b6f-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e8b6f-117">JSON representation</span></span>

<span data-ttu-id="e8b6f-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e8b6f-118">The following is a JSON representation of the resource.</span></span>

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
