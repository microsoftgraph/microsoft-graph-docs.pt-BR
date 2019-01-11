---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Vídeo
localization_priority: Normal
ms.openlocfilehash: 3883dd494304409b76d10781039424267ada85f0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866630"
---
# <a name="video-resource-type"></a><span data-ttu-id="91823-102">Tipo de recurso Video</span><span class="sxs-lookup"><span data-stu-id="91823-102">Video resource type</span></span>

> <span data-ttu-id="91823-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="91823-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91823-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="91823-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="91823-105">O recurso **Video** agrupa itens de dados relacionados a vídeos em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="91823-105">The **Video** resource groups video-related data items into a single structure.</span></span>

<span data-ttu-id="91823-p102">Se um [**DriveItem**](driveitem.md) tiver uma faceta **video** não nula, o item representa um vídeo. As propriedades do recurso **Video** são preenchidas extraindo-se os metadados do arquivo.</span><span class="sxs-lookup"><span data-stu-id="91823-p102">If a [**DriveItem**](driveitem.md) has a non-null **video** facet, the item represents a video file. The properties of the **Video** resource are populated by extracting metadata from the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="91823-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="91823-108">JSON representation</span></span>

<span data-ttu-id="91823-109">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="91823-109">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="91823-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="91823-110">Properties</span></span>

| <span data-ttu-id="91823-111">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="91823-111">Property name</span></span>             | <span data-ttu-id="91823-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="91823-112">Type</span></span>   | <span data-ttu-id="91823-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="91823-113">Description</span></span>
|:--------------------------|:-------|:----------------------------------------
| <span data-ttu-id="91823-114">**audioBitsPerSample**</span><span class="sxs-lookup"><span data-stu-id="91823-114">**audioBitsPerSample**</span></span>    | <span data-ttu-id="91823-115">Int32</span><span class="sxs-lookup"><span data-stu-id="91823-115">Int32</span></span>  | <span data-ttu-id="91823-116">Número de bits áudio por amostra.</span><span class="sxs-lookup"><span data-stu-id="91823-116">Number of audio bits per sample.</span></span>
| <span data-ttu-id="91823-117">**audioChannels**</span><span class="sxs-lookup"><span data-stu-id="91823-117">**audioChannels**</span></span>         | <span data-ttu-id="91823-118">Int32</span><span class="sxs-lookup"><span data-stu-id="91823-118">Int32</span></span>  | <span data-ttu-id="91823-119">Número de canais de áudio.</span><span class="sxs-lookup"><span data-stu-id="91823-119">Number of audio channels.</span></span>
| <span data-ttu-id="91823-120">**audioFormat**</span><span class="sxs-lookup"><span data-stu-id="91823-120">**audioFormat**</span></span>           | <span data-ttu-id="91823-121">string</span><span class="sxs-lookup"><span data-stu-id="91823-121">string</span></span> | <span data-ttu-id="91823-122">Nome do formato áudio (AAC, MP3, etc.).</span><span class="sxs-lookup"><span data-stu-id="91823-122">Name of the audio format (AAC, MP3, etc.).</span></span>
| <span data-ttu-id="91823-123">**audioSamplesPerSecond**</span><span class="sxs-lookup"><span data-stu-id="91823-123">**audioSamplesPerSecond**</span></span> | <span data-ttu-id="91823-124">Int32</span><span class="sxs-lookup"><span data-stu-id="91823-124">Int32</span></span>  | <span data-ttu-id="91823-125">Número de amostras de áudio por segundo.</span><span class="sxs-lookup"><span data-stu-id="91823-125">Number of audio samples per second.</span></span>
| <span data-ttu-id="91823-126">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="91823-126">**bitrate**</span></span>               | <span data-ttu-id="91823-127">Int32</span><span class="sxs-lookup"><span data-stu-id="91823-127">Int32</span></span>  | <span data-ttu-id="91823-128">Taxa de bits do vídeo em bits por segundo.</span><span class="sxs-lookup"><span data-stu-id="91823-128">Bit rate of the video in bits per second.</span></span>
| <span data-ttu-id="91823-129">**duration**</span><span class="sxs-lookup"><span data-stu-id="91823-129">**duration**</span></span>              | <span data-ttu-id="91823-130">Int64</span><span class="sxs-lookup"><span data-stu-id="91823-130">Int64</span></span>  | <span data-ttu-id="91823-131">Duração do arquivo em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="91823-131">Duration of the file in milliseconds.</span></span>
| <span data-ttu-id="91823-132">**fourCC**</span><span class="sxs-lookup"><span data-stu-id="91823-132">**fourCC**</span></span>                | <span data-ttu-id="91823-133">string</span><span class="sxs-lookup"><span data-stu-id="91823-133">string</span></span> | <span data-ttu-id="91823-134">Nome do formato de vídeo "Código de quatro caracteres".</span><span class="sxs-lookup"><span data-stu-id="91823-134">"Four character code" name of the video format.</span></span>
| <span data-ttu-id="91823-135">**framerate**</span><span class="sxs-lookup"><span data-stu-id="91823-135">**framerate**</span></span>             | <span data-ttu-id="91823-136">double</span><span class="sxs-lookup"><span data-stu-id="91823-136">double</span></span> | <span data-ttu-id="91823-137">Taxa de quadros do vídeo.</span><span class="sxs-lookup"><span data-stu-id="91823-137">Frame rate of the video.</span></span>
| <span data-ttu-id="91823-138">**height**</span><span class="sxs-lookup"><span data-stu-id="91823-138">**height**</span></span>                | <span data-ttu-id="91823-139">Int32</span><span class="sxs-lookup"><span data-stu-id="91823-139">Int32</span></span>  | <span data-ttu-id="91823-140">A altura do vídeo em pixels.</span><span class="sxs-lookup"><span data-stu-id="91823-140">Height of the video, in pixels.</span></span>
| <span data-ttu-id="91823-141">**width**</span><span class="sxs-lookup"><span data-stu-id="91823-141">**width**</span></span>                 | <span data-ttu-id="91823-142">Int32</span><span class="sxs-lookup"><span data-stu-id="91823-142">Int32</span></span>  | <span data-ttu-id="91823-143">A largura do vídeo em pixels.</span><span class="sxs-lookup"><span data-stu-id="91823-143">Width of the video, in pixels.</span></span>

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="91823-144">Comentários</span><span class="sxs-lookup"><span data-stu-id="91823-144">Remarks</span></span>

<span data-ttu-id="91823-145">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="91823-145">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>





<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": ""
}-->
