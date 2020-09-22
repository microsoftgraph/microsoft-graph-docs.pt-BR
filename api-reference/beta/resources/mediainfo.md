---
title: tipo de recurso mediaInfo
description: As informações de mídia usadas em ações para prompts.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b7e2b5fb0e00a7b173e1e14962b614fcca5382f5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971739"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="2bb40-103">tipo de recurso mediaInfo</span><span class="sxs-lookup"><span data-stu-id="2bb40-103">mediaInfo resource type</span></span>

<span data-ttu-id="2bb40-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bb40-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2bb40-105">As informações de mídia usadas em ações para prompts.</span><span class="sxs-lookup"><span data-stu-id="2bb40-105">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="2bb40-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2bb40-106">Properties</span></span>
| <span data-ttu-id="2bb40-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2bb40-107">Property</span></span>       | <span data-ttu-id="2bb40-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="2bb40-108">Type</span></span>    | <span data-ttu-id="2bb40-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2bb40-109">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="2bb40-110">resourceId</span><span class="sxs-lookup"><span data-stu-id="2bb40-110">resourceId</span></span>     | <span data-ttu-id="2bb40-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2bb40-111">String</span></span>  | <span data-ttu-id="2bb40-112">Opcional, usada para identificar exclusivamente o recurso.</span><span class="sxs-lookup"><span data-stu-id="2bb40-112">Optional, used to uniquely identity the resource.</span></span> <span data-ttu-id="2bb40-113">Se for passado, a URI do prompt será armazenada em cache para esta ResourceId como chave.</span><span class="sxs-lookup"><span data-stu-id="2bb40-113">If passed the prompt uri will be cached against this resourceId as key.</span></span> |
| <span data-ttu-id="2bb40-114">URI</span><span class="sxs-lookup"><span data-stu-id="2bb40-114">uri</span></span>            | <span data-ttu-id="2bb40-115">String</span><span class="sxs-lookup"><span data-stu-id="2bb40-115">String</span></span>  | <span data-ttu-id="2bb40-116">Caminho para o prompt a ser reproduzido.</span><span class="sxs-lookup"><span data-stu-id="2bb40-116">Path to the prompt to be played.</span></span> <span data-ttu-id="2bb40-117">Atualmente, somente os exemplos de arquivo Wave (. wav), de canal único e 16 bits com uma taxa de amostragem de 16.000 (16 kHz) só têm suporte.</span><span class="sxs-lookup"><span data-stu-id="2bb40-117">Currently only Wave file (.wav) format, single-channel, 16-bit samples with a 16,000 (16KHz) sampling rate is only supported.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="2bb40-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2bb40-118">JSON representation</span></span>

<span data-ttu-id="2bb40-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2bb40-119">The following is a JSON representation of the resource.</span></span>

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


