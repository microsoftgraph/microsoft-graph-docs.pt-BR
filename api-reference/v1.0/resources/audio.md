---
author: ananmishr
ms.date: 09/10/2017
title: Áudio
localization_priority: Normal
ms.prod: microsoft-teams
description: O recurso Audio agrupa propriedades relacionadas a áudio em um item em uma estrutura simples.
doc_type: resourcePageType
ms.openlocfilehash: 2bb74ec0a51c2ec95b477695afc80be48626eee8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988517"
---
# <a name="audio-facet"></a><span data-ttu-id="0bf70-103">Faceta Audio</span><span class="sxs-lookup"><span data-stu-id="0bf70-103">Audio facet</span></span>

<span data-ttu-id="0bf70-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bf70-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0bf70-105">O recurso **Audio** agrupa propriedades relacionadas a áudio em um item em uma estrutura simples.</span><span class="sxs-lookup"><span data-stu-id="0bf70-105">The **Audio** resource groups audio-related properties on an item into a single structure.</span></span>

<span data-ttu-id="0bf70-p101">Se um [**DriveItem**](driveitem.md) tiver uma faceta **audio** não nula, o item representará um arquivo de áudio. As propriedades do recurso **Áudio** são preenchidas extraindo-se os metadados do arquivo.</span><span class="sxs-lookup"><span data-stu-id="0bf70-p101">If a [**DriveItem**](driveitem.md) has a non-null **audio** facet, the item represents an audio file. The properties of the **Audio** resource are populated by extracting metadata from the file.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="0bf70-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0bf70-108">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="0bf70-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0bf70-109">Properties</span></span>

| <span data-ttu-id="0bf70-110">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="0bf70-110">Property name</span></span>         | <span data-ttu-id="0bf70-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="0bf70-111">Type</span></span>    | <span data-ttu-id="0bf70-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bf70-112">Description</span></span>                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| <span data-ttu-id="0bf70-113">**album**</span><span class="sxs-lookup"><span data-stu-id="0bf70-113">**album**</span></span>             | <span data-ttu-id="0bf70-114">string</span><span class="sxs-lookup"><span data-stu-id="0bf70-114">string</span></span>  | <span data-ttu-id="0bf70-115">O título do álbum deste arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="0bf70-115">The title of the album for this audio file.</span></span>                          |
| <span data-ttu-id="0bf70-116">**albumArtist**</span><span class="sxs-lookup"><span data-stu-id="0bf70-116">**albumArtist**</span></span>       | <span data-ttu-id="0bf70-117">string</span><span class="sxs-lookup"><span data-stu-id="0bf70-117">string</span></span>  | <span data-ttu-id="0bf70-118">Artista nomeado no álbum para o arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="0bf70-118">The artist named on the album for the audio file.</span></span>                    |
| <span data-ttu-id="0bf70-119">**artist**</span><span class="sxs-lookup"><span data-stu-id="0bf70-119">**artist**</span></span>            | <span data-ttu-id="0bf70-120">string</span><span class="sxs-lookup"><span data-stu-id="0bf70-120">string</span></span>  | <span data-ttu-id="0bf70-121">O artista do arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="0bf70-121">The performing artist for the audio file.</span></span>                            |
| <span data-ttu-id="0bf70-122">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="0bf70-122">**bitrate**</span></span>           | <span data-ttu-id="0bf70-123">Int64</span><span class="sxs-lookup"><span data-stu-id="0bf70-123">Int64</span></span>   | <span data-ttu-id="0bf70-124">Taxa de bits expressa em kbps.</span><span class="sxs-lookup"><span data-stu-id="0bf70-124">Bitrate expressed in kbps.</span></span>                                           |
| <span data-ttu-id="0bf70-125">**composers**</span><span class="sxs-lookup"><span data-stu-id="0bf70-125">**composers**</span></span>         | <span data-ttu-id="0bf70-126">string</span><span class="sxs-lookup"><span data-stu-id="0bf70-126">string</span></span>  | <span data-ttu-id="0bf70-127">O nome do compositor do arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="0bf70-127">The name of the composer of the audio file.</span></span>                          |
| <span data-ttu-id="0bf70-128">**copyright**</span><span class="sxs-lookup"><span data-stu-id="0bf70-128">**copyright**</span></span>         | <span data-ttu-id="0bf70-129">string</span><span class="sxs-lookup"><span data-stu-id="0bf70-129">string</span></span>  | <span data-ttu-id="0bf70-130">Informações de direitos autorais para o arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="0bf70-130">Copyright information for the audio file.</span></span>                            |
| <span data-ttu-id="0bf70-131">**disc**</span><span class="sxs-lookup"><span data-stu-id="0bf70-131">**disc**</span></span>              | <span data-ttu-id="0bf70-132">Int16</span><span class="sxs-lookup"><span data-stu-id="0bf70-132">Int16</span></span>   | <span data-ttu-id="0bf70-133">O número do disco do qual este arquivo de áudio é proveniente.</span><span class="sxs-lookup"><span data-stu-id="0bf70-133">The number of the disc this audio file came from.</span></span>                    |
| <span data-ttu-id="0bf70-134">**discCount**</span><span class="sxs-lookup"><span data-stu-id="0bf70-134">**discCount**</span></span>         | <span data-ttu-id="0bf70-135">Int16</span><span class="sxs-lookup"><span data-stu-id="0bf70-135">Int16</span></span>   | <span data-ttu-id="0bf70-136">O número total de discos neste álbum.</span><span class="sxs-lookup"><span data-stu-id="0bf70-136">The total number of discs in this album.</span></span>                             |
| <span data-ttu-id="0bf70-137">**duration**</span><span class="sxs-lookup"><span data-stu-id="0bf70-137">**duration**</span></span>          | <span data-ttu-id="0bf70-138">Int64</span><span class="sxs-lookup"><span data-stu-id="0bf70-138">Int64</span></span>   | <span data-ttu-id="0bf70-139">Duração do arquivo de áudio, expressa em milissegundos</span><span class="sxs-lookup"><span data-stu-id="0bf70-139">Duration of the audio file, expressed in milliseconds</span></span>                |
| <span data-ttu-id="0bf70-140">**genre**</span><span class="sxs-lookup"><span data-stu-id="0bf70-140">**genre**</span></span>             | <span data-ttu-id="0bf70-141">string</span><span class="sxs-lookup"><span data-stu-id="0bf70-141">string</span></span>  | <span data-ttu-id="0bf70-142">O gênero deste arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="0bf70-142">The genre of this audio file.</span></span>                                        |
| <span data-ttu-id="0bf70-143">**hasDrm**</span><span class="sxs-lookup"><span data-stu-id="0bf70-143">**hasDrm**</span></span>            | <span data-ttu-id="0bf70-144">booliano</span><span class="sxs-lookup"><span data-stu-id="0bf70-144">boolean</span></span> | <span data-ttu-id="0bf70-145">Indica se o arquivo está protegido com o gerenciamento de direitos digitais.</span><span class="sxs-lookup"><span data-stu-id="0bf70-145">Indicates if the file is protected with digital rights management.</span></span>   |
| <span data-ttu-id="0bf70-146">**isVariableBitrate**</span><span class="sxs-lookup"><span data-stu-id="0bf70-146">**isVariableBitrate**</span></span> | <span data-ttu-id="0bf70-147">booliano</span><span class="sxs-lookup"><span data-stu-id="0bf70-147">boolean</span></span> | <span data-ttu-id="0bf70-148">Indica se o arquivo é codificado com uma taxa de bits variável.</span><span class="sxs-lookup"><span data-stu-id="0bf70-148">Indicates if the file is encoded with a variable bitrate.</span></span>            |
| <span data-ttu-id="0bf70-149">**title**</span><span class="sxs-lookup"><span data-stu-id="0bf70-149">**title**</span></span>             | <span data-ttu-id="0bf70-150">string</span><span class="sxs-lookup"><span data-stu-id="0bf70-150">string</span></span>  | <span data-ttu-id="0bf70-151">O título do arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="0bf70-151">The title of the audio file.</span></span>                                         |
| <span data-ttu-id="0bf70-152">**track**</span><span class="sxs-lookup"><span data-stu-id="0bf70-152">**track**</span></span>             | <span data-ttu-id="0bf70-153">Int32</span><span class="sxs-lookup"><span data-stu-id="0bf70-153">Int32</span></span>   | <span data-ttu-id="0bf70-154">O número da faixa no disco original para este arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="0bf70-154">The number of the track on the original disc for this audio file.</span></span>    |
| <span data-ttu-id="0bf70-155">**trackCount**</span><span class="sxs-lookup"><span data-stu-id="0bf70-155">**trackCount**</span></span>        | <span data-ttu-id="0bf70-156">Int32</span><span class="sxs-lookup"><span data-stu-id="0bf70-156">Int32</span></span>   | <span data-ttu-id="0bf70-157">O número total de faixas no disco original para este arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="0bf70-157">The total number of tracks on the original disc for this audio file.</span></span> |
| <span data-ttu-id="0bf70-158">**year**</span><span class="sxs-lookup"><span data-stu-id="0bf70-158">**year**</span></span>              | <span data-ttu-id="0bf70-159">Int32</span><span class="sxs-lookup"><span data-stu-id="0bf70-159">Int32</span></span>   | <span data-ttu-id="0bf70-160">O ano em que o arquivo de áudio foi gravado.</span><span class="sxs-lookup"><span data-stu-id="0bf70-160">The year the audio file was recorded.</span></span>                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="0bf70-161">Comentários</span><span class="sxs-lookup"><span data-stu-id="0bf70-161">Remarks</span></span>

<span data-ttu-id="0bf70-162">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="0bf70-162">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio"
} -->

