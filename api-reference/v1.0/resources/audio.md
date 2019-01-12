---
author: VinodRavichandran
ms.date: 09/10/2017
title: Áudio
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8265850a6194938cc3547d081c71256bb2aa9251
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990303"
---
# <a name="audio-facet"></a><span data-ttu-id="ed6cf-102">Faceta Audio</span><span class="sxs-lookup"><span data-stu-id="ed6cf-102">Audio facet</span></span>

<span data-ttu-id="ed6cf-103">O recurso **Audio** agrupa propriedades relacionadas a áudio em um item em uma estrutura simples.</span><span class="sxs-lookup"><span data-stu-id="ed6cf-103">The **Audio** resource groups audio-related properties on an item into a single structure.</span></span>

<span data-ttu-id="ed6cf-p101">Se um [**DriveItem**](driveitem.md) tiver uma faceta **audio** não nula, o item representará um arquivo de áudio. As propriedades do recurso **Áudio** são preenchidas extraindo-se os metadados do arquivo.</span><span class="sxs-lookup"><span data-stu-id="ed6cf-p101">If a [**DriveItem**](driveitem.md) has a non-null **audio** facet, the item represents an audio file. The properties of the **Audio** resource are populated by extracting metadata from the file.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="ed6cf-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed6cf-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="ed6cf-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed6cf-107">Properties</span></span>

| <span data-ttu-id="ed6cf-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="ed6cf-108">Property name</span></span>         | <span data-ttu-id="ed6cf-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed6cf-109">Type</span></span>    | <span data-ttu-id="ed6cf-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed6cf-110">Description</span></span>                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| <span data-ttu-id="ed6cf-111">**album**</span><span class="sxs-lookup"><span data-stu-id="ed6cf-111">**album**</span></span>             | <span data-ttu-id="ed6cf-112">string</span><span class="sxs-lookup"><span data-stu-id="ed6cf-112">string</span></span>  | <span data-ttu-id="ed6cf-113">O título do álbum deste arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="ed6cf-113">The title of the album for this audio file.</span></span>                          |
| <span data-ttu-id="ed6cf-114">**albumArtist**</span><span class="sxs-lookup"><span data-stu-id="ed6cf-114">**albumArtist**</span></span>       | <span data-ttu-id="ed6cf-115">string</span><span class="sxs-lookup"><span data-stu-id="ed6cf-115">string</span></span>  | <span data-ttu-id="ed6cf-116">Artista nomeado no álbum para o arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="ed6cf-116">The artist named on the album for the audio file.</span></span>                    |
| <span data-ttu-id="ed6cf-117">**artist**</span><span class="sxs-lookup"><span data-stu-id="ed6cf-117">**artist**</span></span>            | <span data-ttu-id="ed6cf-118">string</span><span class="sxs-lookup"><span data-stu-id="ed6cf-118">string</span></span>  | <span data-ttu-id="ed6cf-119">O artista do arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="ed6cf-119">The performing artist for the audio file.</span></span>                            |
| <span data-ttu-id="ed6cf-120">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="ed6cf-120">**bitrate**</span></span>           | <span data-ttu-id="ed6cf-121">Int64</span><span class="sxs-lookup"><span data-stu-id="ed6cf-121">Int64</span></span>   | <span data-ttu-id="ed6cf-122">Taxa de bits expressa em kbps.</span><span class="sxs-lookup"><span data-stu-id="ed6cf-122">Bitrate expressed in kbps.</span></span>                                           |
| <span data-ttu-id="ed6cf-123">**composers**</span><span class="sxs-lookup"><span data-stu-id="ed6cf-123">**composers**</span></span>         | <span data-ttu-id="ed6cf-124">string</span><span class="sxs-lookup"><span data-stu-id="ed6cf-124">string</span></span>  | <span data-ttu-id="ed6cf-125">O nome do compositor do arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="ed6cf-125">The name of the composer of the audio file.</span></span>                          |
| <span data-ttu-id="ed6cf-126">**copyright**</span><span class="sxs-lookup"><span data-stu-id="ed6cf-126">**copyright**</span></span>         | <span data-ttu-id="ed6cf-127">string</span><span class="sxs-lookup"><span data-stu-id="ed6cf-127">string</span></span>  | <span data-ttu-id="ed6cf-128">Informações de direitos autorais para o arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="ed6cf-128">Copyright information for the audio file.</span></span>                            |
| <span data-ttu-id="ed6cf-129">**disc**</span><span class="sxs-lookup"><span data-stu-id="ed6cf-129">**disc**</span></span>              | <span data-ttu-id="ed6cf-130">Int16</span><span class="sxs-lookup"><span data-stu-id="ed6cf-130">Int16</span></span>   | <span data-ttu-id="ed6cf-131">O número do disco do qual este arquivo de áudio é proveniente.</span><span class="sxs-lookup"><span data-stu-id="ed6cf-131">The number of the disc this audio file came from.</span></span>                    |
| <span data-ttu-id="ed6cf-132">**discCount**</span><span class="sxs-lookup"><span data-stu-id="ed6cf-132">**discCount**</span></span>         | <span data-ttu-id="ed6cf-133">Int16</span><span class="sxs-lookup"><span data-stu-id="ed6cf-133">Int16</span></span>   | <span data-ttu-id="ed6cf-134">O número total de discos neste álbum.</span><span class="sxs-lookup"><span data-stu-id="ed6cf-134">The total number of discs in this album.</span></span>                             |
| <span data-ttu-id="ed6cf-135">**duration**</span><span class="sxs-lookup"><span data-stu-id="ed6cf-135">**duration**</span></span>          | <span data-ttu-id="ed6cf-136">Int64</span><span class="sxs-lookup"><span data-stu-id="ed6cf-136">Int64</span></span>   | <span data-ttu-id="ed6cf-137">Duração do arquivo de áudio, expressa em milissegundos</span><span class="sxs-lookup"><span data-stu-id="ed6cf-137">Duration of the audio file, expressed in milliseconds</span></span>                |
| <span data-ttu-id="ed6cf-138">**genre**</span><span class="sxs-lookup"><span data-stu-id="ed6cf-138">**genre**</span></span>             | <span data-ttu-id="ed6cf-139">string</span><span class="sxs-lookup"><span data-stu-id="ed6cf-139">string</span></span>  | <span data-ttu-id="ed6cf-140">O gênero deste arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="ed6cf-140">The genre of this audio file.</span></span>                                        |
| <span data-ttu-id="ed6cf-141">**hasDrm**</span><span class="sxs-lookup"><span data-stu-id="ed6cf-141">**hasDrm**</span></span>            | <span data-ttu-id="ed6cf-142">booliano</span><span class="sxs-lookup"><span data-stu-id="ed6cf-142">boolean</span></span> | <span data-ttu-id="ed6cf-143">Indica se o arquivo está protegido com o gerenciamento de direitos digitais.</span><span class="sxs-lookup"><span data-stu-id="ed6cf-143">Indicates if the file is protected with digital rights management.</span></span>   |
| <span data-ttu-id="ed6cf-144">**isVariableBitrate**</span><span class="sxs-lookup"><span data-stu-id="ed6cf-144">**isVariableBitrate**</span></span> | <span data-ttu-id="ed6cf-145">booliano</span><span class="sxs-lookup"><span data-stu-id="ed6cf-145">boolean</span></span> | <span data-ttu-id="ed6cf-146">Indica se o arquivo é codificado com uma taxa de bits variável.</span><span class="sxs-lookup"><span data-stu-id="ed6cf-146">Indicates if the file is encoded with a variable bitrate.</span></span>            |
| <span data-ttu-id="ed6cf-147">**title**</span><span class="sxs-lookup"><span data-stu-id="ed6cf-147">**title**</span></span>             | <span data-ttu-id="ed6cf-148">string</span><span class="sxs-lookup"><span data-stu-id="ed6cf-148">string</span></span>  | <span data-ttu-id="ed6cf-149">O título do arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="ed6cf-149">The title of the audio file.</span></span>                                         |
| <span data-ttu-id="ed6cf-150">**track**</span><span class="sxs-lookup"><span data-stu-id="ed6cf-150">**track**</span></span>             | <span data-ttu-id="ed6cf-151">Int32</span><span class="sxs-lookup"><span data-stu-id="ed6cf-151">Int32</span></span>   | <span data-ttu-id="ed6cf-152">O número da faixa no disco original para este arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="ed6cf-152">The number of the track on the original disc for this audio file.</span></span>    |
| <span data-ttu-id="ed6cf-153">**trackCount**</span><span class="sxs-lookup"><span data-stu-id="ed6cf-153">**trackCount**</span></span>        | <span data-ttu-id="ed6cf-154">Int32</span><span class="sxs-lookup"><span data-stu-id="ed6cf-154">Int32</span></span>   | <span data-ttu-id="ed6cf-155">O número total de faixas no disco original para este arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="ed6cf-155">The total number of tracks on the original disc for this audio file.</span></span> |
| <span data-ttu-id="ed6cf-156">**year**</span><span class="sxs-lookup"><span data-stu-id="ed6cf-156">**year**</span></span>              | <span data-ttu-id="ed6cf-157">Int32</span><span class="sxs-lookup"><span data-stu-id="ed6cf-157">Int32</span></span>   | <span data-ttu-id="ed6cf-158">O ano em que o arquivo de áudio foi gravado.</span><span class="sxs-lookup"><span data-stu-id="ed6cf-158">The year the audio file was recorded.</span></span>                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="ed6cf-159">Comentários</span><span class="sxs-lookup"><span data-stu-id="ed6cf-159">Remarks</span></span>

<span data-ttu-id="ed6cf-160">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="ed6cf-160">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio"
} -->
