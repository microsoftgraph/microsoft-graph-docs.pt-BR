---
author: VinodRavichandran
ms.date: 09/10/2017
title: Áudio
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b4ff9e98b3024184298da144f90665ba2f192fef
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642272"
---
# <a name="audio-facet"></a><span data-ttu-id="79a5b-102">Faceta Audio</span><span class="sxs-lookup"><span data-stu-id="79a5b-102">Audio facet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79a5b-103">O recurso **Audio** agrupa propriedades relacionadas a áudio em um item em uma estrutura simples.</span><span class="sxs-lookup"><span data-stu-id="79a5b-103">The **Audio** resource groups audio-related properties on an item into a single structure.</span></span>

<span data-ttu-id="79a5b-p101">Se um [**DriveItem**](driveitem.md) tiver uma faceta **audio** não nula, o item representará um arquivo de áudio. As propriedades do recurso **Áudio** são preenchidas extraindo-se os metadados do arquivo.</span><span class="sxs-lookup"><span data-stu-id="79a5b-p101">If a [**DriveItem**](driveitem.md) has a non-null **audio** facet, the item represents an audio file. The properties of the **Audio** resource are populated by extracting metadata from the file.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="79a5b-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="79a5b-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.audio" } -->
```json
{
  "album": "string",
  "albumArtist": "string",
  "artist": "string",
  "bitrate": 128,
  "composers": "string",
  "copyright": "string",
  "disc": 0,
  "discCount": 0,
  "duration": 567,
  "genre": "string",
  "hasDrm": false,
  "isVariableBitrate": false,
  "title": "string",
  "track": 1,
  "trackCount": 16,
  "year": 2014
}
```

## <a name="properties"></a><span data-ttu-id="79a5b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="79a5b-107">Properties</span></span>

| <span data-ttu-id="79a5b-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="79a5b-108">Property name</span></span>         | <span data-ttu-id="79a5b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="79a5b-109">Type</span></span>    | <span data-ttu-id="79a5b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="79a5b-110">Description</span></span>                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| <span data-ttu-id="79a5b-111">**album**</span><span class="sxs-lookup"><span data-stu-id="79a5b-111">**album**</span></span>             | <span data-ttu-id="79a5b-112">string</span><span class="sxs-lookup"><span data-stu-id="79a5b-112">string</span></span>  | <span data-ttu-id="79a5b-113">O título do álbum deste arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="79a5b-113">The title of the album for this audio file.</span></span>                          |
| <span data-ttu-id="79a5b-114">**albumArtist**</span><span class="sxs-lookup"><span data-stu-id="79a5b-114">**albumArtist**</span></span>       | <span data-ttu-id="79a5b-115">string</span><span class="sxs-lookup"><span data-stu-id="79a5b-115">string</span></span>  | <span data-ttu-id="79a5b-116">Artista nomeado no álbum para o arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="79a5b-116">The artist named on the album for the audio file.</span></span>                    |
| <span data-ttu-id="79a5b-117">**artist**</span><span class="sxs-lookup"><span data-stu-id="79a5b-117">**artist**</span></span>            | <span data-ttu-id="79a5b-118">string</span><span class="sxs-lookup"><span data-stu-id="79a5b-118">string</span></span>  | <span data-ttu-id="79a5b-119">O artista do arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="79a5b-119">The performing artist for the audio file.</span></span>                            |
| <span data-ttu-id="79a5b-120">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="79a5b-120">**bitrate**</span></span>           | <span data-ttu-id="79a5b-121">Int32</span><span class="sxs-lookup"><span data-stu-id="79a5b-121">Int32</span></span>   | <span data-ttu-id="79a5b-122">Taxa de bits expressa em kbps.</span><span class="sxs-lookup"><span data-stu-id="79a5b-122">Bitrate expressed in kbps.</span></span>                                           |
| <span data-ttu-id="79a5b-123">**composers**</span><span class="sxs-lookup"><span data-stu-id="79a5b-123">**composers**</span></span>         | <span data-ttu-id="79a5b-124">string</span><span class="sxs-lookup"><span data-stu-id="79a5b-124">string</span></span>  | <span data-ttu-id="79a5b-125">O nome do compositor do arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="79a5b-125">The name of the composer of the audio file.</span></span>                          |
| <span data-ttu-id="79a5b-126">**copyright**</span><span class="sxs-lookup"><span data-stu-id="79a5b-126">**copyright**</span></span>         | <span data-ttu-id="79a5b-127">string</span><span class="sxs-lookup"><span data-stu-id="79a5b-127">string</span></span>  | <span data-ttu-id="79a5b-128">Informações de direitos autorais para o arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="79a5b-128">Copyright information for the audio file.</span></span>                            |
| <span data-ttu-id="79a5b-129">**disc**</span><span class="sxs-lookup"><span data-stu-id="79a5b-129">**disc**</span></span>              | <span data-ttu-id="79a5b-130">Int32</span><span class="sxs-lookup"><span data-stu-id="79a5b-130">Int32</span></span>   | <span data-ttu-id="79a5b-131">O número do disco do qual este arquivo de áudio é proveniente.</span><span class="sxs-lookup"><span data-stu-id="79a5b-131">The number of the disc this audio file came from.</span></span>                    |
| <span data-ttu-id="79a5b-132">**discCount**</span><span class="sxs-lookup"><span data-stu-id="79a5b-132">**discCount**</span></span>         | <span data-ttu-id="79a5b-133">Int32</span><span class="sxs-lookup"><span data-stu-id="79a5b-133">Int32</span></span>   | <span data-ttu-id="79a5b-134">O número total de discos neste álbum.</span><span class="sxs-lookup"><span data-stu-id="79a5b-134">The total number of discs in this album.</span></span>                             |
| <span data-ttu-id="79a5b-135">**duration**</span><span class="sxs-lookup"><span data-stu-id="79a5b-135">**duration**</span></span>          | <span data-ttu-id="79a5b-136">Int64</span><span class="sxs-lookup"><span data-stu-id="79a5b-136">Int64</span></span>   | <span data-ttu-id="79a5b-137">Duração do arquivo de áudio, expressa em milissegundos</span><span class="sxs-lookup"><span data-stu-id="79a5b-137">Duration of the audio file, expressed in milliseconds</span></span>                |
| <span data-ttu-id="79a5b-138">**genre**</span><span class="sxs-lookup"><span data-stu-id="79a5b-138">**genre**</span></span>             | <span data-ttu-id="79a5b-139">string</span><span class="sxs-lookup"><span data-stu-id="79a5b-139">string</span></span>  | <span data-ttu-id="79a5b-140">O gênero deste arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="79a5b-140">The genre of this audio file.</span></span>                                        |
| <span data-ttu-id="79a5b-141">**hasDrm**</span><span class="sxs-lookup"><span data-stu-id="79a5b-141">**hasDrm**</span></span>            | <span data-ttu-id="79a5b-142">booliano</span><span class="sxs-lookup"><span data-stu-id="79a5b-142">boolean</span></span> | <span data-ttu-id="79a5b-143">Indica se o arquivo está protegido com o gerenciamento de direitos digitais.</span><span class="sxs-lookup"><span data-stu-id="79a5b-143">Indicates if the file is protected with digital rights management.</span></span>   |
| <span data-ttu-id="79a5b-144">**isVariableBitrate**</span><span class="sxs-lookup"><span data-stu-id="79a5b-144">**isVariableBitrate**</span></span> | <span data-ttu-id="79a5b-145">booliano</span><span class="sxs-lookup"><span data-stu-id="79a5b-145">boolean</span></span> | <span data-ttu-id="79a5b-146">Indica se o arquivo é codificado com uma taxa de bits variável.</span><span class="sxs-lookup"><span data-stu-id="79a5b-146">Indicates if the file is encoded with a variable bitrate.</span></span>            |
| <span data-ttu-id="79a5b-147">**title**</span><span class="sxs-lookup"><span data-stu-id="79a5b-147">**title**</span></span>             | <span data-ttu-id="79a5b-148">string</span><span class="sxs-lookup"><span data-stu-id="79a5b-148">string</span></span>  | <span data-ttu-id="79a5b-149">O título do arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="79a5b-149">The title of the audio file.</span></span>                                         |
| <span data-ttu-id="79a5b-150">**track**</span><span class="sxs-lookup"><span data-stu-id="79a5b-150">**track**</span></span>             | <span data-ttu-id="79a5b-151">Int32</span><span class="sxs-lookup"><span data-stu-id="79a5b-151">Int32</span></span>   | <span data-ttu-id="79a5b-152">O número da faixa no disco original para este arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="79a5b-152">The number of the track on the original disc for this audio file.</span></span>    |
| <span data-ttu-id="79a5b-153">**trackCount**</span><span class="sxs-lookup"><span data-stu-id="79a5b-153">**trackCount**</span></span>        | <span data-ttu-id="79a5b-154">Int32</span><span class="sxs-lookup"><span data-stu-id="79a5b-154">Int32</span></span>   | <span data-ttu-id="79a5b-155">O número total de faixas no disco original para este arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="79a5b-155">The total number of tracks on the original disc for this audio file.</span></span> |
| <span data-ttu-id="79a5b-156">**year**</span><span class="sxs-lookup"><span data-stu-id="79a5b-156">**year**</span></span>              | <span data-ttu-id="79a5b-157">Int32</span><span class="sxs-lookup"><span data-stu-id="79a5b-157">Int32</span></span>   | <span data-ttu-id="79a5b-158">O ano em que o arquivo de áudio foi gravado.</span><span class="sxs-lookup"><span data-stu-id="79a5b-158">The year the audio file was recorded.</span></span>                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="79a5b-159">Comentários</span><span class="sxs-lookup"><span data-stu-id="79a5b-159">Remarks</span></span>

<span data-ttu-id="79a5b-160">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="79a5b-160">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio",
  "suppressions": [
    "Error: /api-reference/beta/resources/audio.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
