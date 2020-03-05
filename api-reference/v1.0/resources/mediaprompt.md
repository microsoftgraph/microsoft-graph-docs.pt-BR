---
title: tipo de recurso mediaPrompt
description: Esse tipo de recurso contém informações sobre o arquivo de áudio a ser reproduzido e outras configurações adicionais.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4bc2f315a2f339d2ef6fe0f4b76b335970b5a642
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447441"
---
# <a name="mediaprompt-resource-type"></a><span data-ttu-id="de398-103">tipo de recurso mediaPrompt</span><span class="sxs-lookup"><span data-stu-id="de398-103">mediaPrompt resource type</span></span>

<span data-ttu-id="de398-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="de398-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="de398-105">Esse tipo de recurso contém informações sobre o arquivo de áudio a ser reproduzido e outras configurações adicionais.</span><span class="sxs-lookup"><span data-stu-id="de398-105">This resource type contains information about the audio file to be played and other additional settings.</span></span>

## <a name="properties"></a><span data-ttu-id="de398-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="de398-106">Properties</span></span>

| <span data-ttu-id="de398-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de398-107">Property</span></span>    | <span data-ttu-id="de398-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="de398-108">Type</span></span>                      | <span data-ttu-id="de398-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="de398-109">Description</span></span>                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| <span data-ttu-id="de398-110">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="de398-110">mediaInfo</span></span>   | [<span data-ttu-id="de398-111">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="de398-111">mediaInfo</span></span>](mediainfo.md) | <span data-ttu-id="de398-112">As informações de mídia</span><span class="sxs-lookup"><span data-stu-id="de398-112">The media information</span></span>                                                           |

## <a name="json-representation"></a><span data-ttu-id="de398-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="de398-113">JSON representation</span></span>

<span data-ttu-id="de398-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="de398-114">The following is a JSON representation of the resource.</span></span>

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
