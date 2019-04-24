---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Vídeo
localization_priority: Normal
ms.openlocfilehash: 1e780c8392316be1f7fcc59f3818085dc462da29
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454020"
---
# <a name="video-resource-type"></a><span data-ttu-id="419d3-102">Tipo de recurso Video</span><span class="sxs-lookup"><span data-stu-id="419d3-102">Video resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="419d3-103">O recurso **Video** agrupa itens de dados relacionados a vídeos em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="419d3-103">The **Video** resource groups video-related data items into a single structure.</span></span>

<span data-ttu-id="419d3-p101">Se um [**DriveItem**](driveitem.md) tiver uma faceta **video** não nula, o item representa um vídeo. As propriedades do recurso **Video** são preenchidas extraindo-se os metadados do arquivo.</span><span class="sxs-lookup"><span data-stu-id="419d3-p101">If a [**DriveItem**](driveitem.md) has a non-null **video** facet, the item represents a video file. The properties of the **Video** resource are populated by extracting metadata from the file.</span></span>

## <a name="json-representation"></a><span data-ttu-id="419d3-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="419d3-106">JSON representation</span></span>

<span data-ttu-id="419d3-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="419d3-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="419d3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="419d3-108">Properties</span></span>

| <span data-ttu-id="419d3-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="419d3-109">Property name</span></span>             | <span data-ttu-id="419d3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="419d3-110">Type</span></span>   | <span data-ttu-id="419d3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="419d3-111">Description</span></span>
|:--------------------------|:-------|:----------------------------------------
| <span data-ttu-id="419d3-112">**audioBitsPerSample**</span><span class="sxs-lookup"><span data-stu-id="419d3-112">**audioBitsPerSample**</span></span>    | <span data-ttu-id="419d3-113">Int32</span><span class="sxs-lookup"><span data-stu-id="419d3-113">Int32</span></span>  | <span data-ttu-id="419d3-114">Número de bits áudio por amostra.</span><span class="sxs-lookup"><span data-stu-id="419d3-114">Number of audio bits per sample.</span></span>
| <span data-ttu-id="419d3-115">**audioChannels**</span><span class="sxs-lookup"><span data-stu-id="419d3-115">**audioChannels**</span></span>         | <span data-ttu-id="419d3-116">Int32</span><span class="sxs-lookup"><span data-stu-id="419d3-116">Int32</span></span>  | <span data-ttu-id="419d3-117">Número de canais de áudio.</span><span class="sxs-lookup"><span data-stu-id="419d3-117">Number of audio channels.</span></span>
| <span data-ttu-id="419d3-118">**audioFormat**</span><span class="sxs-lookup"><span data-stu-id="419d3-118">**audioFormat**</span></span>           | <span data-ttu-id="419d3-119">string</span><span class="sxs-lookup"><span data-stu-id="419d3-119">string</span></span> | <span data-ttu-id="419d3-120">Nome do formato áudio (AAC, MP3, etc.).</span><span class="sxs-lookup"><span data-stu-id="419d3-120">Name of the audio format (AAC, MP3, etc.).</span></span>
| <span data-ttu-id="419d3-121">**audioSamplesPerSecond**</span><span class="sxs-lookup"><span data-stu-id="419d3-121">**audioSamplesPerSecond**</span></span> | <span data-ttu-id="419d3-122">Int32</span><span class="sxs-lookup"><span data-stu-id="419d3-122">Int32</span></span>  | <span data-ttu-id="419d3-123">Número de amostras de áudio por segundo.</span><span class="sxs-lookup"><span data-stu-id="419d3-123">Number of audio samples per second.</span></span>
| <span data-ttu-id="419d3-124">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="419d3-124">**bitrate**</span></span>               | <span data-ttu-id="419d3-125">Int32</span><span class="sxs-lookup"><span data-stu-id="419d3-125">Int32</span></span>  | <span data-ttu-id="419d3-126">Taxa de bits do vídeo em bits por segundo.</span><span class="sxs-lookup"><span data-stu-id="419d3-126">Bit rate of the video in bits per second.</span></span>
| <span data-ttu-id="419d3-127">**duration**</span><span class="sxs-lookup"><span data-stu-id="419d3-127">**duration**</span></span>              | <span data-ttu-id="419d3-128">Int64</span><span class="sxs-lookup"><span data-stu-id="419d3-128">Int64</span></span>  | <span data-ttu-id="419d3-129">Duração do arquivo em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="419d3-129">Duration of the file in milliseconds.</span></span>
| <span data-ttu-id="419d3-130">**fourCC**</span><span class="sxs-lookup"><span data-stu-id="419d3-130">**fourCC**</span></span>                | <span data-ttu-id="419d3-131">string</span><span class="sxs-lookup"><span data-stu-id="419d3-131">string</span></span> | <span data-ttu-id="419d3-132">Nome do formato de vídeo "Código de quatro caracteres".</span><span class="sxs-lookup"><span data-stu-id="419d3-132">"Four character code" name of the video format.</span></span>
| <span data-ttu-id="419d3-133">**framerate**</span><span class="sxs-lookup"><span data-stu-id="419d3-133">**framerate**</span></span>             | <span data-ttu-id="419d3-134">double</span><span class="sxs-lookup"><span data-stu-id="419d3-134">double</span></span> | <span data-ttu-id="419d3-135">Taxa de quadros do vídeo.</span><span class="sxs-lookup"><span data-stu-id="419d3-135">Frame rate of the video.</span></span>
| <span data-ttu-id="419d3-136">**height**</span><span class="sxs-lookup"><span data-stu-id="419d3-136">**height**</span></span>                | <span data-ttu-id="419d3-137">Int32</span><span class="sxs-lookup"><span data-stu-id="419d3-137">Int32</span></span>  | <span data-ttu-id="419d3-138">A altura do vídeo em pixels.</span><span class="sxs-lookup"><span data-stu-id="419d3-138">Height of the video, in pixels.</span></span>
| <span data-ttu-id="419d3-139">**width**</span><span class="sxs-lookup"><span data-stu-id="419d3-139">**width**</span></span>                 | <span data-ttu-id="419d3-140">Int32</span><span class="sxs-lookup"><span data-stu-id="419d3-140">Int32</span></span>  | <span data-ttu-id="419d3-141">A largura do vídeo em pixels.</span><span class="sxs-lookup"><span data-stu-id="419d3-141">Width of the video, in pixels.</span></span>

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="419d3-142">Comentários</span><span class="sxs-lookup"><span data-stu-id="419d3-142">Remarks</span></span>

<span data-ttu-id="419d3-143">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="419d3-143">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>





<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The video facet provides information about the properties of a video file.",
  "keywords": "bitrate,duration,size,video",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/video.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
