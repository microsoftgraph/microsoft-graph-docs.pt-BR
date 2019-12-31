---
author: ananmishr
description: O recurso Audio agrupa propriedades relacionadas a áudio em um item em uma estrutura simples.
ms.date: 09/10/2017
title: Áudio
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 539afcd93ed2f8d9d5b1a136edefa5a69fd2e4bd
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913139"
---
# <a name="audio-facet"></a><span data-ttu-id="b1545-103">Faceta Audio</span><span class="sxs-lookup"><span data-stu-id="b1545-103">Audio facet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1545-104">O recurso **Audio** agrupa propriedades relacionadas a áudio em um item em uma estrutura simples.</span><span class="sxs-lookup"><span data-stu-id="b1545-104">The **Audio** resource groups audio-related properties on an item into a single structure.</span></span>

<span data-ttu-id="b1545-p101">Se um [**DriveItem**](driveitem.md) tiver uma faceta **audio** não nula, o item representará um arquivo de áudio. As propriedades do recurso **Áudio** são preenchidas extraindo-se os metadados do arquivo.</span><span class="sxs-lookup"><span data-stu-id="b1545-p101">If a [**DriveItem**](driveitem.md) has a non-null **audio** facet, the item represents an audio file. The properties of the **Audio** resource are populated by extracting metadata from the file.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="b1545-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1545-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="b1545-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1545-108">Properties</span></span>

| <span data-ttu-id="b1545-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="b1545-109">Property name</span></span>         | <span data-ttu-id="b1545-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1545-110">Type</span></span>    | <span data-ttu-id="b1545-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1545-111">Description</span></span>                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| <span data-ttu-id="b1545-112">**album**</span><span class="sxs-lookup"><span data-stu-id="b1545-112">**album**</span></span>             | <span data-ttu-id="b1545-113">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1545-113">string</span></span>  | <span data-ttu-id="b1545-114">O título do álbum deste arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="b1545-114">The title of the album for this audio file.</span></span>                          |
| <span data-ttu-id="b1545-115">**albumArtist**</span><span class="sxs-lookup"><span data-stu-id="b1545-115">**albumArtist**</span></span>       | <span data-ttu-id="b1545-116">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1545-116">string</span></span>  | <span data-ttu-id="b1545-117">Artista nomeado no álbum para o arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="b1545-117">The artist named on the album for the audio file.</span></span>                    |
| <span data-ttu-id="b1545-118">**artist**</span><span class="sxs-lookup"><span data-stu-id="b1545-118">**artist**</span></span>            | <span data-ttu-id="b1545-119">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1545-119">string</span></span>  | <span data-ttu-id="b1545-120">O artista do arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="b1545-120">The performing artist for the audio file.</span></span>                            |
| <span data-ttu-id="b1545-121">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="b1545-121">**bitrate**</span></span>           | <span data-ttu-id="b1545-122">Int32</span><span class="sxs-lookup"><span data-stu-id="b1545-122">Int32</span></span>   | <span data-ttu-id="b1545-123">Taxa de bits expressa em kbps.</span><span class="sxs-lookup"><span data-stu-id="b1545-123">Bitrate expressed in kbps.</span></span>                                           |
| <span data-ttu-id="b1545-124">**composers**</span><span class="sxs-lookup"><span data-stu-id="b1545-124">**composers**</span></span>         | <span data-ttu-id="b1545-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1545-125">string</span></span>  | <span data-ttu-id="b1545-126">O nome do compositor do arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="b1545-126">The name of the composer of the audio file.</span></span>                          |
| <span data-ttu-id="b1545-127">**copyright**</span><span class="sxs-lookup"><span data-stu-id="b1545-127">**copyright**</span></span>         | <span data-ttu-id="b1545-128">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1545-128">string</span></span>  | <span data-ttu-id="b1545-129">Informações de direitos autorais para o arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="b1545-129">Copyright information for the audio file.</span></span>                            |
| <span data-ttu-id="b1545-130">**disc**</span><span class="sxs-lookup"><span data-stu-id="b1545-130">**disc**</span></span>              | <span data-ttu-id="b1545-131">Int32</span><span class="sxs-lookup"><span data-stu-id="b1545-131">Int32</span></span>   | <span data-ttu-id="b1545-132">O número do disco do qual este arquivo de áudio é proveniente.</span><span class="sxs-lookup"><span data-stu-id="b1545-132">The number of the disc this audio file came from.</span></span>                    |
| <span data-ttu-id="b1545-133">**discCount**</span><span class="sxs-lookup"><span data-stu-id="b1545-133">**discCount**</span></span>         | <span data-ttu-id="b1545-134">Int32</span><span class="sxs-lookup"><span data-stu-id="b1545-134">Int32</span></span>   | <span data-ttu-id="b1545-135">O número total de discos neste álbum.</span><span class="sxs-lookup"><span data-stu-id="b1545-135">The total number of discs in this album.</span></span>                             |
| <span data-ttu-id="b1545-136">**duration**</span><span class="sxs-lookup"><span data-stu-id="b1545-136">**duration**</span></span>          | <span data-ttu-id="b1545-137">Int64</span><span class="sxs-lookup"><span data-stu-id="b1545-137">Int64</span></span>   | <span data-ttu-id="b1545-138">Duração do arquivo de áudio, expressa em milissegundos</span><span class="sxs-lookup"><span data-stu-id="b1545-138">Duration of the audio file, expressed in milliseconds</span></span>                |
| <span data-ttu-id="b1545-139">**genre**</span><span class="sxs-lookup"><span data-stu-id="b1545-139">**genre**</span></span>             | <span data-ttu-id="b1545-140">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1545-140">string</span></span>  | <span data-ttu-id="b1545-141">O gênero deste arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="b1545-141">The genre of this audio file.</span></span>                                        |
| <span data-ttu-id="b1545-142">**hasDrm**</span><span class="sxs-lookup"><span data-stu-id="b1545-142">**hasDrm**</span></span>            | <span data-ttu-id="b1545-143">booliano</span><span class="sxs-lookup"><span data-stu-id="b1545-143">boolean</span></span> | <span data-ttu-id="b1545-144">Indica se o arquivo está protegido com o gerenciamento de direitos digitais.</span><span class="sxs-lookup"><span data-stu-id="b1545-144">Indicates if the file is protected with digital rights management.</span></span>   |
| <span data-ttu-id="b1545-145">**isVariableBitrate**</span><span class="sxs-lookup"><span data-stu-id="b1545-145">**isVariableBitrate**</span></span> | <span data-ttu-id="b1545-146">booliano</span><span class="sxs-lookup"><span data-stu-id="b1545-146">boolean</span></span> | <span data-ttu-id="b1545-147">Indica se o arquivo é codificado com uma taxa de bits variável.</span><span class="sxs-lookup"><span data-stu-id="b1545-147">Indicates if the file is encoded with a variable bitrate.</span></span>            |
| <span data-ttu-id="b1545-148">**title**</span><span class="sxs-lookup"><span data-stu-id="b1545-148">**title**</span></span>             | <span data-ttu-id="b1545-149">string</span><span class="sxs-lookup"><span data-stu-id="b1545-149">string</span></span>  | <span data-ttu-id="b1545-150">O título do arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="b1545-150">The title of the audio file.</span></span>                                         |
| <span data-ttu-id="b1545-151">**track**</span><span class="sxs-lookup"><span data-stu-id="b1545-151">**track**</span></span>             | <span data-ttu-id="b1545-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b1545-152">Int32</span></span>   | <span data-ttu-id="b1545-153">O número da faixa no disco original para este arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="b1545-153">The number of the track on the original disc for this audio file.</span></span>    |
| <span data-ttu-id="b1545-154">**trackCount**</span><span class="sxs-lookup"><span data-stu-id="b1545-154">**trackCount**</span></span>        | <span data-ttu-id="b1545-155">Int32</span><span class="sxs-lookup"><span data-stu-id="b1545-155">Int32</span></span>   | <span data-ttu-id="b1545-156">O número total de faixas no disco original para este arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="b1545-156">The total number of tracks on the original disc for this audio file.</span></span> |
| <span data-ttu-id="b1545-157">**year**</span><span class="sxs-lookup"><span data-stu-id="b1545-157">**year**</span></span>              | <span data-ttu-id="b1545-158">Int32</span><span class="sxs-lookup"><span data-stu-id="b1545-158">Int32</span></span>   | <span data-ttu-id="b1545-159">O ano em que o arquivo de áudio foi gravado.</span><span class="sxs-lookup"><span data-stu-id="b1545-159">The year the audio file was recorded.</span></span>                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="b1545-160">Comentários</span><span class="sxs-lookup"><span data-stu-id="b1545-160">Remarks</span></span>

<span data-ttu-id="b1545-161">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="b1545-161">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio",
  "suppressions": []
}
-->
