---
author: JeremyKelley
description: O recurso Video agrupa itens de dados relacionados a vídeos em uma única estrutura.
ms.date: 09/10/2017
title: Vídeo
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: b80d36ce35a950fa20424124b20cba34c19307c3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519467"
---
# <a name="video-resource-type"></a><span data-ttu-id="a8440-103">Tipo de recurso Video</span><span class="sxs-lookup"><span data-stu-id="a8440-103">Video resource type</span></span>

<span data-ttu-id="a8440-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a8440-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8440-105">O recurso **Video** agrupa itens de dados relacionados a vídeos em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="a8440-105">The **Video** resource groups video-related data items into a single structure.</span></span>

<span data-ttu-id="a8440-p101">Se um [**DriveItem**](driveitem.md) tiver uma faceta **video** não nula, o item representa um vídeo. As propriedades do recurso **Video** são preenchidas extraindo-se os metadados do arquivo.</span><span class="sxs-lookup"><span data-stu-id="a8440-p101">If a [**DriveItem**](driveitem.md) has a non-null **video** facet, the item represents a video file. The properties of the **Video** resource are populated by extracting metadata from the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8440-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a8440-108">JSON representation</span></span>

<span data-ttu-id="a8440-109">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="a8440-109">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="a8440-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a8440-110">Properties</span></span>

| <span data-ttu-id="a8440-111">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="a8440-111">Property name</span></span>             | <span data-ttu-id="a8440-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8440-112">Type</span></span>   | <span data-ttu-id="a8440-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8440-113">Description</span></span>
|:--------------------------|:-------|:----------------------------------------
| <span data-ttu-id="a8440-114">**audioBitsPerSample**</span><span class="sxs-lookup"><span data-stu-id="a8440-114">**audioBitsPerSample**</span></span>    | <span data-ttu-id="a8440-115">Int32</span><span class="sxs-lookup"><span data-stu-id="a8440-115">Int32</span></span>  | <span data-ttu-id="a8440-116">Número de bits áudio por amostra.</span><span class="sxs-lookup"><span data-stu-id="a8440-116">Number of audio bits per sample.</span></span>
| <span data-ttu-id="a8440-117">**audioChannels**</span><span class="sxs-lookup"><span data-stu-id="a8440-117">**audioChannels**</span></span>         | <span data-ttu-id="a8440-118">Int32</span><span class="sxs-lookup"><span data-stu-id="a8440-118">Int32</span></span>  | <span data-ttu-id="a8440-119">Número de canais de áudio.</span><span class="sxs-lookup"><span data-stu-id="a8440-119">Number of audio channels.</span></span>
| <span data-ttu-id="a8440-120">**audioFormat**</span><span class="sxs-lookup"><span data-stu-id="a8440-120">**audioFormat**</span></span>           | <span data-ttu-id="a8440-121">string</span><span class="sxs-lookup"><span data-stu-id="a8440-121">string</span></span> | <span data-ttu-id="a8440-122">Nome do formato áudio (AAC, MP3, etc.).</span><span class="sxs-lookup"><span data-stu-id="a8440-122">Name of the audio format (AAC, MP3, etc.).</span></span>
| <span data-ttu-id="a8440-123">**audioSamplesPerSecond**</span><span class="sxs-lookup"><span data-stu-id="a8440-123">**audioSamplesPerSecond**</span></span> | <span data-ttu-id="a8440-124">Int32</span><span class="sxs-lookup"><span data-stu-id="a8440-124">Int32</span></span>  | <span data-ttu-id="a8440-125">Número de amostras de áudio por segundo.</span><span class="sxs-lookup"><span data-stu-id="a8440-125">Number of audio samples per second.</span></span>
| <span data-ttu-id="a8440-126">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="a8440-126">**bitrate**</span></span>               | <span data-ttu-id="a8440-127">Int32</span><span class="sxs-lookup"><span data-stu-id="a8440-127">Int32</span></span>  | <span data-ttu-id="a8440-128">Taxa de bits do vídeo em bits por segundo.</span><span class="sxs-lookup"><span data-stu-id="a8440-128">Bit rate of the video in bits per second.</span></span>
| <span data-ttu-id="a8440-129">**duration**</span><span class="sxs-lookup"><span data-stu-id="a8440-129">**duration**</span></span>              | <span data-ttu-id="a8440-130">Int64</span><span class="sxs-lookup"><span data-stu-id="a8440-130">Int64</span></span>  | <span data-ttu-id="a8440-131">Duração do arquivo em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="a8440-131">Duration of the file in milliseconds.</span></span>
| <span data-ttu-id="a8440-132">**fourCC**</span><span class="sxs-lookup"><span data-stu-id="a8440-132">**fourCC**</span></span>                | <span data-ttu-id="a8440-133">string</span><span class="sxs-lookup"><span data-stu-id="a8440-133">string</span></span> | <span data-ttu-id="a8440-134">Nome do formato de vídeo "Código de quatro caracteres".</span><span class="sxs-lookup"><span data-stu-id="a8440-134">"Four character code" name of the video format.</span></span>
| <span data-ttu-id="a8440-135">**framerate**</span><span class="sxs-lookup"><span data-stu-id="a8440-135">**framerate**</span></span>             | <span data-ttu-id="a8440-136">double</span><span class="sxs-lookup"><span data-stu-id="a8440-136">double</span></span> | <span data-ttu-id="a8440-137">Taxa de quadros do vídeo.</span><span class="sxs-lookup"><span data-stu-id="a8440-137">Frame rate of the video.</span></span>
| <span data-ttu-id="a8440-138">**height**</span><span class="sxs-lookup"><span data-stu-id="a8440-138">**height**</span></span>                | <span data-ttu-id="a8440-139">Int32</span><span class="sxs-lookup"><span data-stu-id="a8440-139">Int32</span></span>  | <span data-ttu-id="a8440-140">A altura do vídeo em pixels.</span><span class="sxs-lookup"><span data-stu-id="a8440-140">Height of the video, in pixels.</span></span>
| <span data-ttu-id="a8440-141">**width**</span><span class="sxs-lookup"><span data-stu-id="a8440-141">**width**</span></span>                 | <span data-ttu-id="a8440-142">Int32</span><span class="sxs-lookup"><span data-stu-id="a8440-142">Int32</span></span>  | <span data-ttu-id="a8440-143">A largura do vídeo em pixels.</span><span class="sxs-lookup"><span data-stu-id="a8440-143">Width of the video, in pixels.</span></span>

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="a8440-144">Comentários</span><span class="sxs-lookup"><span data-stu-id="a8440-144">Remarks</span></span>

<span data-ttu-id="a8440-145">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="a8440-145">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>





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
