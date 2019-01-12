---
author: VinodRavichandran
ms.date: 09/10/2017
title: Áudio
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b88fbbcd11a4cbeff56c870225d7b0bef4b32346
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985372"
---
# <a name="audio-facet"></a><span data-ttu-id="3530c-102">Faceta Audio</span><span class="sxs-lookup"><span data-stu-id="3530c-102">Audio facet</span></span>

> <span data-ttu-id="3530c-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3530c-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3530c-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3530c-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3530c-105">O recurso **Audio** agrupa propriedades relacionadas a áudio em um item em uma estrutura simples.</span><span class="sxs-lookup"><span data-stu-id="3530c-105">The **Audio** resource groups audio-related properties on an item into a single structure.</span></span>

<span data-ttu-id="3530c-p102">Se um [**DriveItem**](driveitem.md) tiver uma faceta **audio** não nula, o item representará um arquivo de áudio. As propriedades do recurso **Áudio** são preenchidas extraindo-se os metadados do arquivo.</span><span class="sxs-lookup"><span data-stu-id="3530c-p102">If a [**DriveItem**](driveitem.md) has a non-null **audio** facet, the item represents an audio file. The properties of the **Audio** resource are populated by extracting metadata from the file.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="3530c-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3530c-108">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="3530c-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3530c-109">Properties</span></span>

| <span data-ttu-id="3530c-110">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="3530c-110">Property name</span></span>         | <span data-ttu-id="3530c-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3530c-111">Type</span></span>    | <span data-ttu-id="3530c-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3530c-112">Description</span></span>                                                          |
|:----------------------|:--------|:---------------------------------------------------------------------|
| <span data-ttu-id="3530c-113">**album**</span><span class="sxs-lookup"><span data-stu-id="3530c-113">**album**</span></span>             | <span data-ttu-id="3530c-114">string</span><span class="sxs-lookup"><span data-stu-id="3530c-114">string</span></span>  | <span data-ttu-id="3530c-115">O título do álbum deste arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="3530c-115">The title of the album for this audio file.</span></span>                          |
| <span data-ttu-id="3530c-116">**albumArtist**</span><span class="sxs-lookup"><span data-stu-id="3530c-116">**albumArtist**</span></span>       | <span data-ttu-id="3530c-117">string</span><span class="sxs-lookup"><span data-stu-id="3530c-117">string</span></span>  | <span data-ttu-id="3530c-118">Artista nomeado no álbum para o arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="3530c-118">The artist named on the album for the audio file.</span></span>                    |
| <span data-ttu-id="3530c-119">**artist**</span><span class="sxs-lookup"><span data-stu-id="3530c-119">**artist**</span></span>            | <span data-ttu-id="3530c-120">string</span><span class="sxs-lookup"><span data-stu-id="3530c-120">string</span></span>  | <span data-ttu-id="3530c-121">O artista do arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="3530c-121">The performing artist for the audio file.</span></span>                            |
| <span data-ttu-id="3530c-122">**bitrate**</span><span class="sxs-lookup"><span data-stu-id="3530c-122">**bitrate**</span></span>           | <span data-ttu-id="3530c-123">Int32</span><span class="sxs-lookup"><span data-stu-id="3530c-123">Int32</span></span>   | <span data-ttu-id="3530c-124">Taxa de bits expressa em kbps.</span><span class="sxs-lookup"><span data-stu-id="3530c-124">Bitrate expressed in kbps.</span></span>                                           |
| <span data-ttu-id="3530c-125">**composers**</span><span class="sxs-lookup"><span data-stu-id="3530c-125">**composers**</span></span>         | <span data-ttu-id="3530c-126">string</span><span class="sxs-lookup"><span data-stu-id="3530c-126">string</span></span>  | <span data-ttu-id="3530c-127">O nome do compositor do arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="3530c-127">The name of the composer of the audio file.</span></span>                          |
| <span data-ttu-id="3530c-128">**copyright**</span><span class="sxs-lookup"><span data-stu-id="3530c-128">**copyright**</span></span>         | <span data-ttu-id="3530c-129">string</span><span class="sxs-lookup"><span data-stu-id="3530c-129">string</span></span>  | <span data-ttu-id="3530c-130">Informações de direitos autorais para o arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="3530c-130">Copyright information for the audio file.</span></span>                            |
| <span data-ttu-id="3530c-131">**disc**</span><span class="sxs-lookup"><span data-stu-id="3530c-131">**disc**</span></span>              | <span data-ttu-id="3530c-132">Int32</span><span class="sxs-lookup"><span data-stu-id="3530c-132">Int32</span></span>   | <span data-ttu-id="3530c-133">O número do disco do qual este arquivo de áudio é proveniente.</span><span class="sxs-lookup"><span data-stu-id="3530c-133">The number of the disc this audio file came from.</span></span>                    |
| <span data-ttu-id="3530c-134">**discCount**</span><span class="sxs-lookup"><span data-stu-id="3530c-134">**discCount**</span></span>         | <span data-ttu-id="3530c-135">Int32</span><span class="sxs-lookup"><span data-stu-id="3530c-135">Int32</span></span>   | <span data-ttu-id="3530c-136">O número total de discos neste álbum.</span><span class="sxs-lookup"><span data-stu-id="3530c-136">The total number of discs in this album.</span></span>                             |
| <span data-ttu-id="3530c-137">**duration**</span><span class="sxs-lookup"><span data-stu-id="3530c-137">**duration**</span></span>          | <span data-ttu-id="3530c-138">Int64</span><span class="sxs-lookup"><span data-stu-id="3530c-138">Int64</span></span>   | <span data-ttu-id="3530c-139">Duração do arquivo de áudio, expressa em milissegundos</span><span class="sxs-lookup"><span data-stu-id="3530c-139">Duration of the audio file, expressed in milliseconds</span></span>                |
| <span data-ttu-id="3530c-140">**genre**</span><span class="sxs-lookup"><span data-stu-id="3530c-140">**genre**</span></span>             | <span data-ttu-id="3530c-141">string</span><span class="sxs-lookup"><span data-stu-id="3530c-141">string</span></span>  | <span data-ttu-id="3530c-142">O gênero deste arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="3530c-142">The genre of this audio file.</span></span>                                        |
| <span data-ttu-id="3530c-143">**hasDrm**</span><span class="sxs-lookup"><span data-stu-id="3530c-143">**hasDrm**</span></span>            | <span data-ttu-id="3530c-144">booliano</span><span class="sxs-lookup"><span data-stu-id="3530c-144">boolean</span></span> | <span data-ttu-id="3530c-145">Indica se o arquivo está protegido com o gerenciamento de direitos digitais.</span><span class="sxs-lookup"><span data-stu-id="3530c-145">Indicates if the file is protected with digital rights management.</span></span>   |
| <span data-ttu-id="3530c-146">**isVariableBitrate**</span><span class="sxs-lookup"><span data-stu-id="3530c-146">**isVariableBitrate**</span></span> | <span data-ttu-id="3530c-147">booliano</span><span class="sxs-lookup"><span data-stu-id="3530c-147">boolean</span></span> | <span data-ttu-id="3530c-148">Indica se o arquivo é codificado com uma taxa de bits variável.</span><span class="sxs-lookup"><span data-stu-id="3530c-148">Indicates if the file is encoded with a variable bitrate.</span></span>            |
| <span data-ttu-id="3530c-149">**title**</span><span class="sxs-lookup"><span data-stu-id="3530c-149">**title**</span></span>             | <span data-ttu-id="3530c-150">string</span><span class="sxs-lookup"><span data-stu-id="3530c-150">string</span></span>  | <span data-ttu-id="3530c-151">O título do arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="3530c-151">The title of the audio file.</span></span>                                         |
| <span data-ttu-id="3530c-152">**track**</span><span class="sxs-lookup"><span data-stu-id="3530c-152">**track**</span></span>             | <span data-ttu-id="3530c-153">Int32</span><span class="sxs-lookup"><span data-stu-id="3530c-153">Int32</span></span>   | <span data-ttu-id="3530c-154">O número da faixa no disco original para este arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="3530c-154">The number of the track on the original disc for this audio file.</span></span>    |
| <span data-ttu-id="3530c-155">**trackCount**</span><span class="sxs-lookup"><span data-stu-id="3530c-155">**trackCount**</span></span>        | <span data-ttu-id="3530c-156">Int32</span><span class="sxs-lookup"><span data-stu-id="3530c-156">Int32</span></span>   | <span data-ttu-id="3530c-157">O número total de faixas no disco original para este arquivo de áudio.</span><span class="sxs-lookup"><span data-stu-id="3530c-157">The total number of tracks on the original disc for this audio file.</span></span> |
| <span data-ttu-id="3530c-158">**year**</span><span class="sxs-lookup"><span data-stu-id="3530c-158">**year**</span></span>              | <span data-ttu-id="3530c-159">Int32</span><span class="sxs-lookup"><span data-stu-id="3530c-159">Int32</span></span>   | <span data-ttu-id="3530c-160">O ano em que o arquivo de áudio foi gravado.</span><span class="sxs-lookup"><span data-stu-id="3530c-160">The year the audio file was recorded.</span></span>                                |

[item-resource]: ../resources/driveitem.md

## <a name="remarks"></a><span data-ttu-id="3530c-161">Comentários</span><span class="sxs-lookup"><span data-stu-id="3530c-161">Remarks</span></span>

<span data-ttu-id="3530c-162">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="3530c-162">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The audio facet provides information about music or audio metadata.",
  "keywords": "music,audio,metadata,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Audio"
} -->
