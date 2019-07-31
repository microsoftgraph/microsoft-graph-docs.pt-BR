---
author: JeremyKelley
description: O recurso Video agrupa itens de dados relacionados a vídeos em uma única estrutura.
ms.date: 09/10/2017
title: Vídeo
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: e93fd4bbd348df3ad31d1be6aa2b1dc73593327a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007358"
---
# <a name="video-resource-type"></a><span data-ttu-id="3ec50-103">Tipo de recurso Video</span><span class="sxs-lookup"><span data-stu-id="3ec50-103">Video resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ec50-104">O recurso **Video** agrupa itens de dados relacionados a vídeos em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="3ec50-104">The **Video** resource groups video-related data items into a single structure.</span></span>

<span data-ttu-id="3ec50-p101">Se um [**DriveItem**](driveitem.md) tiver uma faceta **video** não nula, o item representa um vídeo. As propriedades do recurso **Video** são preenchidas extraindo-se os metadados do arquivo.</span><span class="sxs-lookup"><span data-stu-id="3ec50-p101">If a [**DriveItem**](driveitem.md) has a non-null **video** facet, the item represents a video file. The properties of the **Video** resource are populated by extracting metadata from the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ec50-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3ec50-107">JSON representation</span></span>

<span data-ttu-id="3ec50-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="3ec50-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.video"
}-->

```json
{
  "audioBitsPerSample": 16,
  "audioChannels": 1,
  "audioFormat": "AAC",
  "audioSamplesPerSecond": 44100,
  "bitrate": 39101896,
  "duration": 8053,
  "fourCC": "H264",
  "height": 1280,
  "width": 720,
  "framerate": 2.75
}
```

## <a name="properties"></a><span data-ttu-id="3ec50-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3ec50-109">Properties</span></span>

| <span data-ttu-id="3ec50-110">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="3ec50-110">Property name</span></span>             | <span data-ttu-id="3ec50-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ec50-111">Type</span></span>   | <span data-ttu-id="3ec50-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ec50-112">Description</span></span>
|:--------------------------|:-------|:----------------------------------------
| <span data-ttu-id="3ec50-113">**audioBitsPerSample**</span><span class="sxs-lookup"><span data-stu-id="3ec50-113">**audioBitsPerSample**</span></span>    | <span data-ttu-id="3ec50-114">Int32</span><span class="sxs-lookup"><span data-stu-id="3ec50-114">Int32</span></span>  | <span data-ttu-id="3ec50-115">Número de bits áudio por amostra.</span><span class="sxs-lookup"><span data-stu-id="3ec50-115">Number of audio bits per sample.</span></span>
| <span data-ttu-id="3ec50-116">**audioChannels**</span><span class="sxs-lookup"><span data-stu-id="3ec50-116">**audioChannels**</span></span>         | <span data-ttu-id="3ec50-117">Int32</span><span class="sxs-lookup"><span data-stu-id="3ec50-117">Int32</span></span>  | <span data-ttu-id="3ec50-118">Número de canais de áudio.</span><span class="sxs-lookup"><span data-stu-id="3ec50-118">Number of audio channels.</span></span>
| <span data-ttu-id="3ec50-119">**audioFormat**</span><span class="sxs-lookup"><span data-stu-id="3ec50-119">**audioFormat**</span></span>           | <span data-ttu-id="3ec50-120">string</span><span class="sxs-lookup"><span data-stu-id="3ec50-120">string</span></span> | <span data-ttu-id="3ec50-121">Nome do formato áudio (AAC, MP3, etc.).</span><span class="sxs-lookup"><span data-stu-id="3ec50-121">Name of the audio format (AAC, MP3, etc.).</span></span>
| <span data-ttu-id="3ec50-122">**audioSamplesPerSecond**</span><span class="sxs-lookup"><span data-stu-id="3ec50-122">**audioSamplesPerSecond**</span></span> | <span data-ttu-id="3ec50-123">Int32</span><span class="sxs-lookup"><span data-stu-id="3ec50-123">Int32</span></span>  | <span data-ttu-id="3ec50-124">Número de amostras de áudio por segundo.</span><span class="sxs-lookup"><span data-stu-id="3ec50-124">Number of audio samples per second.</span></span>
| <span data-ttu-id="3ec50-125">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="3ec50-125">**bitrate**</span></span>               | <span data-ttu-id="3ec50-126">Int32</span><span class="sxs-lookup"><span data-stu-id="3ec50-126">Int32</span></span>  | <span data-ttu-id="3ec50-127">Taxa de bits do vídeo em bits por segundo.</span><span class="sxs-lookup"><span data-stu-id="3ec50-127">Bit rate of the video in bits per second.</span></span>
| <span data-ttu-id="3ec50-128">**duration**</span><span class="sxs-lookup"><span data-stu-id="3ec50-128">**duration**</span></span>              | <span data-ttu-id="3ec50-129">Int64</span><span class="sxs-lookup"><span data-stu-id="3ec50-129">Int64</span></span>  | <span data-ttu-id="3ec50-130">Duração do arquivo em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="3ec50-130">Duration of the file in milliseconds.</span></span>
| <span data-ttu-id="3ec50-131">**fourCC**</span><span class="sxs-lookup"><span data-stu-id="3ec50-131">**fourCC**</span></span>                | <span data-ttu-id="3ec50-132">string</span><span class="sxs-lookup"><span data-stu-id="3ec50-132">string</span></span> | <span data-ttu-id="3ec50-133">Nome do formato de vídeo "Código de quatro caracteres".</span><span class="sxs-lookup"><span data-stu-id="3ec50-133">"Four character code" name of the video format.</span></span>
| <span data-ttu-id="3ec50-134">**framerate**</span><span class="sxs-lookup"><span data-stu-id="3ec50-134">**framerate**</span></span>             | <span data-ttu-id="3ec50-135">double</span><span class="sxs-lookup"><span data-stu-id="3ec50-135">double</span></span> | <span data-ttu-id="3ec50-136">Taxa de quadros do vídeo.</span><span class="sxs-lookup"><span data-stu-id="3ec50-136">Frame rate of the video.</span></span>
| <span data-ttu-id="3ec50-137">**height**</span><span class="sxs-lookup"><span data-stu-id="3ec50-137">**height**</span></span>                | <span data-ttu-id="3ec50-138">Int32</span><span class="sxs-lookup"><span data-stu-id="3ec50-138">Int32</span></span>  | <span data-ttu-id="3ec50-139">A altura do vídeo em pixels.</span><span class="sxs-lookup"><span data-stu-id="3ec50-139">Height of the video, in pixels.</span></span>
| <span data-ttu-id="3ec50-140">**width**</span><span class="sxs-lookup"><span data-stu-id="3ec50-140">**width**</span></span>                 | <span data-ttu-id="3ec50-141">Int32</span><span class="sxs-lookup"><span data-stu-id="3ec50-141">Int32</span></span>  | <span data-ttu-id="3ec50-142">A largura do vídeo em pixels.</span><span class="sxs-lookup"><span data-stu-id="3ec50-142">Width of the video, in pixels.</span></span>

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="3ec50-143">Comentários</span><span class="sxs-lookup"><span data-stu-id="3ec50-143">Remarks</span></span>

<span data-ttu-id="3ec50-144">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="3ec50-144">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>





<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
