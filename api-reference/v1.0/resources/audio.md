---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "Áudio"
ms.openlocfilehash: 43b9999ecfb472a82e00a12ca820fdf8548eec64
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="audio-facet"></a><span data-ttu-id="2a6a6-102">Faceta Audio</span><span class="sxs-lookup"><span data-stu-id="2a6a6-102">Audio facet</span></span>

<span data-ttu-id="2a6a6-103">O recurso **Audio** agrupa propriedades relacionadas a áudio em um item em uma estrutura simples.</span><span class="sxs-lookup"><span data-stu-id="2a6a6-103">The **Audio** resource groups audio-related properties on an item into a single structure.</span></span>

<span data-ttu-id="2a6a6-104">Se um [**DriveItem**](driveitem.md) tiver uma faceta **audio** não nula, o item representará um arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="2a6a6-104">If a [**DriveItem**](driveitem.md) has a non-null **audio** facet, the item represents an audio file. The properties of the Audio resource are populated by extracting metadata from the file.</span></span>
<span data-ttu-id="2a6a6-105">As propriedades do recurso **Audio** são preenchidas extraindo-se os metadados do arquivo.</span><span class="sxs-lookup"><span data-stu-id="2a6a6-105">If a DriveItem has a non-null audio facet, the item represents an audio file. The properties of the **Audio** resource are populated by extracting metadata from the file.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="2a6a6-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2a6a6-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="2a6a6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2a6a6-107">Properties</span></span>

| <span data-ttu-id="2a6a6-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="2a6a6-108">Property name</span></span>         | <span data-ttu-id="2a6a6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2a6a6-109">Type</span></span>    | <span data-ttu-id="2a6a6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a6a6-110">Description</span></span>                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| <span data-ttu-id="2a6a6-111">**album**</span><span class="sxs-lookup"><span data-stu-id="2a6a6-111">**album**</span></span>             | <span data-ttu-id="2a6a6-112">string</span><span class="sxs-lookup"><span data-stu-id="2a6a6-112">string</span></span>  | <span data-ttu-id="2a6a6-113">O título do álbum deste arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="2a6a6-113">The title of the album for this audio file.</span></span>                          |
| <span data-ttu-id="2a6a6-114">**albumArtist**</span><span class="sxs-lookup"><span data-stu-id="2a6a6-114">**albumArtist**</span></span>       | <span data-ttu-id="2a6a6-115">string</span><span class="sxs-lookup"><span data-stu-id="2a6a6-115">string</span></span>  | <span data-ttu-id="2a6a6-116">Artista nomeado no álbum para o arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="2a6a6-116">The artist named on the album for the audio file.</span></span>                    |
| <span data-ttu-id="2a6a6-117">**artist**</span><span class="sxs-lookup"><span data-stu-id="2a6a6-117">**artist**</span></span>            | <span data-ttu-id="2a6a6-118">string</span><span class="sxs-lookup"><span data-stu-id="2a6a6-118">string</span></span>  | <span data-ttu-id="2a6a6-119">O artista do arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="2a6a6-119">The performing artist for the audio file.</span></span>                            |
| <span data-ttu-id="2a6a6-120">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="2a6a6-120">**bitrate**</span></span>           | <span data-ttu-id="2a6a6-121">Int32</span><span class="sxs-lookup"><span data-stu-id="2a6a6-121">Int32</span></span>   | <span data-ttu-id="2a6a6-122">Taxa de bits expressa em kbps.</span><span class="sxs-lookup"><span data-stu-id="2a6a6-122">Bitrate expressed in kbps.</span></span>                                           |
| <span data-ttu-id="2a6a6-123">**composers**</span><span class="sxs-lookup"><span data-stu-id="2a6a6-123">**composers**</span></span>         | <span data-ttu-id="2a6a6-124">string</span><span class="sxs-lookup"><span data-stu-id="2a6a6-124">string</span></span>  | <span data-ttu-id="2a6a6-125">O nome do compositor do arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="2a6a6-125">The name of the composer of the audio file.</span></span>                          |
| <span data-ttu-id="2a6a6-126">**copyright**</span><span class="sxs-lookup"><span data-stu-id="2a6a6-126">**copyright**</span></span>         | <span data-ttu-id="2a6a6-127">string</span><span class="sxs-lookup"><span data-stu-id="2a6a6-127">string</span></span>  | <span data-ttu-id="2a6a6-128">Informações de direitos autorais para o arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="2a6a6-128">Copyright information for the audio file.</span></span>                            |
| <span data-ttu-id="2a6a6-129">**disc**</span><span class="sxs-lookup"><span data-stu-id="2a6a6-129">**disc**</span></span>              | <span data-ttu-id="2a6a6-130">Int32</span><span class="sxs-lookup"><span data-stu-id="2a6a6-130">Int32</span></span>   | <span data-ttu-id="2a6a6-131">O número do disco do qual este arquivo de áudio é proveniente.</span><span class="sxs-lookup"><span data-stu-id="2a6a6-131">The number of the disc this audio file came from.</span></span>                    |
| <span data-ttu-id="2a6a6-132">**discCount**</span><span class="sxs-lookup"><span data-stu-id="2a6a6-132">**discCount**</span></span>         | <span data-ttu-id="2a6a6-133">Int32</span><span class="sxs-lookup"><span data-stu-id="2a6a6-133">Int32</span></span>   | <span data-ttu-id="2a6a6-134">O número total de discos neste álbum.</span><span class="sxs-lookup"><span data-stu-id="2a6a6-134">The total number of discs in this album.</span></span>                             |
| <span data-ttu-id="2a6a6-135">**duration**</span><span class="sxs-lookup"><span data-stu-id="2a6a6-135">**duration**</span></span>          | <span data-ttu-id="2a6a6-136">Int64</span><span class="sxs-lookup"><span data-stu-id="2a6a6-136">Int64</span></span>   | <span data-ttu-id="2a6a6-137">Duração do arquivo de áudio, expressa em milissegundos</span><span class="sxs-lookup"><span data-stu-id="2a6a6-137">Duration of the audio file, expressed in milliseconds</span></span>                |
| <span data-ttu-id="2a6a6-138">**genre**</span><span class="sxs-lookup"><span data-stu-id="2a6a6-138">**genre**</span></span>             | <span data-ttu-id="2a6a6-139">string</span><span class="sxs-lookup"><span data-stu-id="2a6a6-139">string</span></span>  | <span data-ttu-id="2a6a6-140">O gênero deste arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="2a6a6-140">The genre of this audio file.</span></span>                                        |
| <span data-ttu-id="2a6a6-141">**hasDrm**</span><span class="sxs-lookup"><span data-stu-id="2a6a6-141">**hasDrm**</span></span>            | <span data-ttu-id="2a6a6-142">booliano</span><span class="sxs-lookup"><span data-stu-id="2a6a6-142">boolean</span></span> | <span data-ttu-id="2a6a6-143">Indica se o arquivo está protegido com o gerenciamento de direitos digitais.</span><span class="sxs-lookup"><span data-stu-id="2a6a6-143">Indicates if the file is protected with digital rights management.</span></span>   |
| <span data-ttu-id="2a6a6-144">**isVariableBitrate**</span><span class="sxs-lookup"><span data-stu-id="2a6a6-144">**isVariableBitrate**</span></span> | <span data-ttu-id="2a6a6-145">booliano</span><span class="sxs-lookup"><span data-stu-id="2a6a6-145">boolean</span></span> | <span data-ttu-id="2a6a6-146">Indica se o arquivo é codificado com uma taxa de bits variável.</span><span class="sxs-lookup"><span data-stu-id="2a6a6-146">Indicates if the file is encoded with a variable bitrate.</span></span>            |
| <span data-ttu-id="2a6a6-147">**title**</span><span class="sxs-lookup"><span data-stu-id="2a6a6-147">**title**</span></span>             | <span data-ttu-id="2a6a6-148">string</span><span class="sxs-lookup"><span data-stu-id="2a6a6-148">string</span></span>  | <span data-ttu-id="2a6a6-149">O título do arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="2a6a6-149">The title of the audio file.</span></span>                                         |
| <span data-ttu-id="2a6a6-150">**track**</span><span class="sxs-lookup"><span data-stu-id="2a6a6-150">**track**</span></span>             | <span data-ttu-id="2a6a6-151">Int32</span><span class="sxs-lookup"><span data-stu-id="2a6a6-151">Int32</span></span>   | <span data-ttu-id="2a6a6-152">O número da faixa no disco original para este arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="2a6a6-152">The number of the track on the original disc for this audio file.</span></span>    |
| <span data-ttu-id="2a6a6-153">**trackCount**</span><span class="sxs-lookup"><span data-stu-id="2a6a6-153">**trackCount**</span></span>        | <span data-ttu-id="2a6a6-154">Int32</span><span class="sxs-lookup"><span data-stu-id="2a6a6-154">Int32</span></span>   | <span data-ttu-id="2a6a6-155">O número total de faixas no disco original para este arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="2a6a6-155">The total number of tracks on the original disc for this audio file.</span></span> |
| <span data-ttu-id="2a6a6-156">**year**</span><span class="sxs-lookup"><span data-stu-id="2a6a6-156">**year**</span></span>              | <span data-ttu-id="2a6a6-157">Int32</span><span class="sxs-lookup"><span data-stu-id="2a6a6-157">Int32</span></span>   | <span data-ttu-id="2a6a6-158">O ano em que o arquivo de áudio foi gravado.</span><span class="sxs-lookup"><span data-stu-id="2a6a6-158">The year the audio file was recorded.</span></span>                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="2a6a6-159">Comentários</span><span class="sxs-lookup"><span data-stu-id="2a6a6-159">Remarks</span></span>

<span data-ttu-id="2a6a6-160">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="2a6a6-160">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio"
} -->
