---
title: tipo de recurso mediaInfo
description: As informações de mídia usadas em ações para prompts.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 20134131dba64ad48effa1c95e5d81ab81102805
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913202"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="b0218-103">tipo de recurso mediaInfo</span><span class="sxs-lookup"><span data-stu-id="b0218-103">mediaInfo resource type</span></span>

<span data-ttu-id="b0218-104">As informações de mídia usadas em ações para prompts.</span><span class="sxs-lookup"><span data-stu-id="b0218-104">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="b0218-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0218-105">Properties</span></span>
| <span data-ttu-id="b0218-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0218-106">Property</span></span>       | <span data-ttu-id="b0218-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0218-107">Type</span></span>    | <span data-ttu-id="b0218-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0218-108">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="b0218-109">resourceId</span><span class="sxs-lookup"><span data-stu-id="b0218-109">resourceId</span></span>     | <span data-ttu-id="b0218-110">String</span><span class="sxs-lookup"><span data-stu-id="b0218-110">String</span></span>  | <span data-ttu-id="b0218-111">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b0218-111">Optional.</span></span> <span data-ttu-id="b0218-112">Usada para identificar exclusivamente o recurso.</span><span class="sxs-lookup"><span data-stu-id="b0218-112">Used to uniquely identity the resource.</span></span> <span data-ttu-id="b0218-113">Se passadas, o URI de prompt será armazenado em cache em relação a este ResourceId como uma chave.</span><span class="sxs-lookup"><span data-stu-id="b0218-113">If passed in, the prompt uri will be cached against this resourceId as a key.</span></span> |
| <span data-ttu-id="b0218-114">URI</span><span class="sxs-lookup"><span data-stu-id="b0218-114">uri</span></span>            | <span data-ttu-id="b0218-115">String</span><span class="sxs-lookup"><span data-stu-id="b0218-115">String</span></span>  | <span data-ttu-id="b0218-116">Caminho para o prompt que será reproduzido.</span><span class="sxs-lookup"><span data-stu-id="b0218-116">Path to the prompt that will be played.</span></span> <span data-ttu-id="b0218-117">O atualmente oferece suporte somente a exemplos de arquivo Wave (. wav), de canal único e 16 bits com uma taxa de amostragem de 16.000 (16 kHz).</span><span class="sxs-lookup"><span data-stu-id="b0218-117">Currently supports only Wave file (.wav) format, single-channel, 16-bit samples with a 16,000 (16KHz) sampling rate.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="b0218-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0218-118">JSON representation</span></span>

<span data-ttu-id="b0218-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0218-119">The following is a JSON representation of the resource.</span></span>

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
