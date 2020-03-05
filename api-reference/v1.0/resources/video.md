---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Vídeo
localization_priority: Normal
description: O recurso Video agrupa itens de dados relacionados a vídeos em uma única estrutura.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 2982dbad8f1e06a2f1288bd499c88c77a4ef2fda
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446762"
---
# <a name="video-resource-type"></a><span data-ttu-id="d1871-103">Tipo de recurso Video</span><span class="sxs-lookup"><span data-stu-id="d1871-103">Video resource type</span></span>

<span data-ttu-id="d1871-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d1871-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d1871-105">O recurso **Video** agrupa itens de dados relacionados a vídeos em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="d1871-105">The **Video** resource groups video-related data items into a single structure.</span></span>

<span data-ttu-id="d1871-p101">Se um [**DriveItem**](driveitem.md) tiver uma faceta **video** não nula, o item representa um vídeo. As propriedades do recurso **Video** são preenchidas extraindo-se os metadados do arquivo.</span><span class="sxs-lookup"><span data-stu-id="d1871-p101">If a [**DriveItem**](driveitem.md) has a non-null **video** facet, the item represents a video file. The properties of the **Video** resource are populated by extracting metadata from the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1871-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d1871-108">JSON representation</span></span>

<span data-ttu-id="d1871-109">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="d1871-109">Here is a JSON representation of the resource</span></span>

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
  "frameRate": 239.877,
  "height": 1280,
  "width": 720
}
```

## <a name="properties"></a><span data-ttu-id="d1871-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d1871-110">Properties</span></span>

| <span data-ttu-id="d1871-111">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="d1871-111">Property name</span></span>             | <span data-ttu-id="d1871-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1871-112">Type</span></span>   | <span data-ttu-id="d1871-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1871-113">Description</span></span>
|:--------------------------|:-------|:----------------------------------------
| <span data-ttu-id="d1871-114">**audioBitsPerSample**</span><span class="sxs-lookup"><span data-stu-id="d1871-114">**audioBitsPerSample**</span></span>    | <span data-ttu-id="d1871-115">Int32</span><span class="sxs-lookup"><span data-stu-id="d1871-115">Int32</span></span>  | <span data-ttu-id="d1871-116">Número de bits áudio por amostra.</span><span class="sxs-lookup"><span data-stu-id="d1871-116">Number of audio bits per sample.</span></span>
| <span data-ttu-id="d1871-117">**audioChannels**</span><span class="sxs-lookup"><span data-stu-id="d1871-117">**audioChannels**</span></span>         | <span data-ttu-id="d1871-118">Int32</span><span class="sxs-lookup"><span data-stu-id="d1871-118">Int32</span></span>  | <span data-ttu-id="d1871-119">Número de canais de áudio.</span><span class="sxs-lookup"><span data-stu-id="d1871-119">Number of audio channels.</span></span>
| <span data-ttu-id="d1871-120">**audioFormat**</span><span class="sxs-lookup"><span data-stu-id="d1871-120">**audioFormat**</span></span>           | <span data-ttu-id="d1871-121">string</span><span class="sxs-lookup"><span data-stu-id="d1871-121">string</span></span> | <span data-ttu-id="d1871-122">Nome do formato áudio (AAC, MP3, etc.).</span><span class="sxs-lookup"><span data-stu-id="d1871-122">Name of the audio format (AAC, MP3, etc.).</span></span>
| <span data-ttu-id="d1871-123">**audioSamplesPerSecond**</span><span class="sxs-lookup"><span data-stu-id="d1871-123">**audioSamplesPerSecond**</span></span> | <span data-ttu-id="d1871-124">Int32</span><span class="sxs-lookup"><span data-stu-id="d1871-124">Int32</span></span>  | <span data-ttu-id="d1871-125">Número de amostras de áudio por segundo.</span><span class="sxs-lookup"><span data-stu-id="d1871-125">Number of audio samples per second.</span></span>
| <span data-ttu-id="d1871-126">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="d1871-126">**bitrate**</span></span>               | <span data-ttu-id="d1871-127">Int32</span><span class="sxs-lookup"><span data-stu-id="d1871-127">Int32</span></span>  | <span data-ttu-id="d1871-128">Taxa de bits do vídeo em bits por segundo.</span><span class="sxs-lookup"><span data-stu-id="d1871-128">Bit rate of the video in bits per second.</span></span>
| <span data-ttu-id="d1871-129">**duration**</span><span class="sxs-lookup"><span data-stu-id="d1871-129">**duration**</span></span>              | <span data-ttu-id="d1871-130">Int64</span><span class="sxs-lookup"><span data-stu-id="d1871-130">Int64</span></span>  | <span data-ttu-id="d1871-131">Duração do arquivo em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="d1871-131">Duration of the file in milliseconds.</span></span>
| <span data-ttu-id="d1871-132">**fourCC**</span><span class="sxs-lookup"><span data-stu-id="d1871-132">**fourCC**</span></span>                | <span data-ttu-id="d1871-133">string</span><span class="sxs-lookup"><span data-stu-id="d1871-133">string</span></span> | <span data-ttu-id="d1871-134">Nome do formato de vídeo "Código de quatro caracteres".</span><span class="sxs-lookup"><span data-stu-id="d1871-134">"Four character code" name of the video format.</span></span>
| <span data-ttu-id="d1871-135">**frameRate**</span><span class="sxs-lookup"><span data-stu-id="d1871-135">**frameRate**</span></span>             | <span data-ttu-id="d1871-136">double</span><span class="sxs-lookup"><span data-stu-id="d1871-136">double</span></span> | <span data-ttu-id="d1871-137">Taxa de quadros do vídeo.</span><span class="sxs-lookup"><span data-stu-id="d1871-137">Frame rate of the video.</span></span>
| <span data-ttu-id="d1871-138">**height**</span><span class="sxs-lookup"><span data-stu-id="d1871-138">**height**</span></span>                | <span data-ttu-id="d1871-139">Int32</span><span class="sxs-lookup"><span data-stu-id="d1871-139">Int32</span></span>  | <span data-ttu-id="d1871-140">A altura do vídeo em pixels.</span><span class="sxs-lookup"><span data-stu-id="d1871-140">Height of the video, in pixels.</span></span>
| <span data-ttu-id="d1871-141">**width**</span><span class="sxs-lookup"><span data-stu-id="d1871-141">**width**</span></span>                 | <span data-ttu-id="d1871-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d1871-142">Int32</span></span>  | <span data-ttu-id="d1871-143">A largura do vídeo em pixels.</span><span class="sxs-lookup"><span data-stu-id="d1871-143">Width of the video, in pixels.</span></span>

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="d1871-144">Comentários</span><span class="sxs-lookup"><span data-stu-id="d1871-144">Remarks</span></span>

<span data-ttu-id="d1871-145">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="d1871-145">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": "Facets/Video"
} -->
