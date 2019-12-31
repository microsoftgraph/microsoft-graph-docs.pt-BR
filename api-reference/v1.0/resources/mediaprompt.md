---
title: tipo de recurso mediaPrompt
description: Esse tipo de recurso contém informações sobre o arquivo de áudio a ser reproduzido e outras configurações adicionais.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0ef83d9645ac4277893ff8c769ecb6e092e3e84d
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913195"
---
# <a name="mediaprompt-resource-type"></a><span data-ttu-id="2ccf4-103">tipo de recurso mediaPrompt</span><span class="sxs-lookup"><span data-stu-id="2ccf4-103">mediaPrompt resource type</span></span>

<span data-ttu-id="2ccf4-104">Esse tipo de recurso contém informações sobre o arquivo de áudio a ser reproduzido e outras configurações adicionais.</span><span class="sxs-lookup"><span data-stu-id="2ccf4-104">This resource type contains information about the audio file to be played and other additional settings.</span></span>

## <a name="properties"></a><span data-ttu-id="2ccf4-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2ccf4-105">Properties</span></span>

| <span data-ttu-id="2ccf4-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ccf4-106">Property</span></span>    | <span data-ttu-id="2ccf4-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ccf4-107">Type</span></span>                      | <span data-ttu-id="2ccf4-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ccf4-108">Description</span></span>                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| <span data-ttu-id="2ccf4-109">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="2ccf4-109">mediaInfo</span></span>   | [<span data-ttu-id="2ccf4-110">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="2ccf4-110">mediaInfo</span></span>](mediainfo.md) | <span data-ttu-id="2ccf4-111">As informações de mídia</span><span class="sxs-lookup"><span data-stu-id="2ccf4-111">The media information</span></span>                                                           |

## <a name="json-representation"></a><span data-ttu-id="2ccf4-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2ccf4-112">JSON representation</span></span>

<span data-ttu-id="2ccf4-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2ccf4-113">The following is a JSON representation of the resource.</span></span>

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
