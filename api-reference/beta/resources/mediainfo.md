---
title: tipo de recurso mediaInfo
description: As informações de mídia usadas em ações para prompts.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ef58bb2ca80ec18a1d11c0e3d2e976e6d7fa2bb9
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006666"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="c07b7-103">tipo de recurso mediaInfo</span><span class="sxs-lookup"><span data-stu-id="c07b7-103">mediaInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c07b7-104">As informações de mídia usadas em ações para prompts.</span><span class="sxs-lookup"><span data-stu-id="c07b7-104">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="c07b7-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c07b7-105">Properties</span></span>
| <span data-ttu-id="c07b7-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c07b7-106">Property</span></span>       | <span data-ttu-id="c07b7-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="c07b7-107">Type</span></span>    | <span data-ttu-id="c07b7-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c07b7-108">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="c07b7-109">resourceId</span><span class="sxs-lookup"><span data-stu-id="c07b7-109">resourceId</span></span>     | <span data-ttu-id="c07b7-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c07b7-110">String</span></span>  | <span data-ttu-id="c07b7-111">Opcional, usada para identificar exclusivamente o recurso.</span><span class="sxs-lookup"><span data-stu-id="c07b7-111">Optional, used to uniquely identity the resource.</span></span> <span data-ttu-id="c07b7-112">Se for passado, a URI do prompt será armazenada em cache para esta ResourceId como chave.</span><span class="sxs-lookup"><span data-stu-id="c07b7-112">If passed the prompt uri will be cached against this resourceId as key.</span></span> |
| <span data-ttu-id="c07b7-113">URI</span><span class="sxs-lookup"><span data-stu-id="c07b7-113">uri</span></span>            | <span data-ttu-id="c07b7-114">String</span><span class="sxs-lookup"><span data-stu-id="c07b7-114">String</span></span>  | <span data-ttu-id="c07b7-115">Caminho para o prompt a ser reproduzido.</span><span class="sxs-lookup"><span data-stu-id="c07b7-115">Path to the prompt to be played.</span></span> <span data-ttu-id="c07b7-116">Atualmente, somente os exemplos de arquivo Wave (. wav), de canal único e 16 bits com uma taxa de amostragem de 16.000 (16 kHz) só têm suporte.</span><span class="sxs-lookup"><span data-stu-id="c07b7-116">Currently only Wave file (.wav) format, single-channel, 16-bit samples with a 16,000 (16KHz) sampling rate is only supported.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="c07b7-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c07b7-117">JSON representation</span></span>

<span data-ttu-id="c07b7-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c07b7-118">The following is a JSON representation of the resource.</span></span>

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
