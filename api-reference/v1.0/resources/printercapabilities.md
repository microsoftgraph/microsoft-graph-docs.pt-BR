---
title: Tipo complexo printerCapabilities
description: Representa os recursos relatados por uma impressora.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 5416cf43e266bab65254ac5aaee1a79c9c3e17be
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516822"
---
# <a name="printercapabilities-resource-type"></a><span data-ttu-id="301b0-103">Tipo de recurso printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="301b0-103">printerCapabilities resource type</span></span>

<span data-ttu-id="301b0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="301b0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="301b0-105">Representa os recursos relatados por um printer/printerShare.</span><span class="sxs-lookup"><span data-stu-id="301b0-105">Represents the capabilities reported by a printer/printerShare.</span></span>

## <a name="properties"></a><span data-ttu-id="301b0-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="301b0-106">Properties</span></span>
| <span data-ttu-id="301b0-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="301b0-107">Property</span></span>     | <span data-ttu-id="301b0-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="301b0-108">Type</span></span>        | <span data-ttu-id="301b0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="301b0-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="301b0-110">contentTypes</span><span class="sxs-lookup"><span data-stu-id="301b0-110">contentTypes</span></span>|<span data-ttu-id="301b0-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="301b0-111">String collection</span></span>|<span data-ttu-id="301b0-112">Uma lista de tipos de conteúdo com suporte (MIME) compatíveis com a impressora.</span><span class="sxs-lookup"><span data-stu-id="301b0-112">A list of supported content (MIME) types that the printer supports.</span></span> <span data-ttu-id="301b0-113">Não é garantido que o serviço Impressão Universal dá suporte à impressão de todos esses tipos mime.</span><span class="sxs-lookup"><span data-stu-id="301b0-113">It is not guaranteed that the Universal Print service supports printing all of these MIME types.</span></span>|
|<span data-ttu-id="301b0-114">isColorPrintingSupported</span><span class="sxs-lookup"><span data-stu-id="301b0-114">isColorPrintingSupported</span></span>|<span data-ttu-id="301b0-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="301b0-115">Boolean</span></span>|<span data-ttu-id="301b0-116">True se a impressão de cores for suportada pela impressora; false caso contrário.</span><span class="sxs-lookup"><span data-stu-id="301b0-116">True if color printing is supported by the printer; false otherwise.</span></span> <span data-ttu-id="301b0-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="301b0-117">Read-only.</span></span>|
|<span data-ttu-id="301b0-118">feedOrientations</span><span class="sxs-lookup"><span data-stu-id="301b0-118">feedOrientations</span></span>|<span data-ttu-id="301b0-119">Coleção printerFeedOrientation</span><span class="sxs-lookup"><span data-stu-id="301b0-119">printerFeedOrientation collection</span></span>|<span data-ttu-id="301b0-120">A lista de orientações de feed que são suportadas pela impressora.</span><span class="sxs-lookup"><span data-stu-id="301b0-120">The list of feed orientations that are supported by the printer.</span></span>|
|<span data-ttu-id="301b0-121">isPageRangeSupported</span><span class="sxs-lookup"><span data-stu-id="301b0-121">isPageRangeSupported</span></span>|<span data-ttu-id="301b0-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="301b0-122">Boolean</span></span>|<span data-ttu-id="301b0-123">True se a impressora dá suporte à impressão por intervalos de página; false caso contrário.</span><span class="sxs-lookup"><span data-stu-id="301b0-123">True if the printer supports printing by page ranges; false otherwise.</span></span>|
|<span data-ttu-id="301b0-124">qualidades</span><span class="sxs-lookup"><span data-stu-id="301b0-124">qualities</span></span>|<span data-ttu-id="301b0-125">[Coleção printQuality](enums.md#printquality-values)</span><span class="sxs-lookup"><span data-stu-id="301b0-125">[printQuality](enums.md#printquality-values) collection</span></span>|<span data-ttu-id="301b0-126">As qualidades de impressão suportadas pela impressora.</span><span class="sxs-lookup"><span data-stu-id="301b0-126">The print qualities supported by the printer.</span></span>|
|<span data-ttu-id="301b0-127">dpis</span><span class="sxs-lookup"><span data-stu-id="301b0-127">dpis</span></span>|<span data-ttu-id="301b0-128">Coleção Int32</span><span class="sxs-lookup"><span data-stu-id="301b0-128">Int32 collection</span></span>|<span data-ttu-id="301b0-129">A lista de resoluções de impressão em DPI que são suportadas pela impressora.</span><span class="sxs-lookup"><span data-stu-id="301b0-129">The list of print resolutions in DPI that are supported by the printer.</span></span>|
|<span data-ttu-id="301b0-130">duplexModes</span><span class="sxs-lookup"><span data-stu-id="301b0-130">duplexModes</span></span>|<span data-ttu-id="301b0-131">[Coleção printDuplexMode](enums.md#printduplexmode-values)</span><span class="sxs-lookup"><span data-stu-id="301b0-131">[printDuplexMode](enums.md#printduplexmode-values) collection</span></span>|<span data-ttu-id="301b0-132">A lista de modos duplex com suporte da impressora.</span><span class="sxs-lookup"><span data-stu-id="301b0-132">The list of duplex modes that are supported by the printer.</span></span> <span data-ttu-id="301b0-133">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="301b0-133">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="301b0-134">queueBufferSizeInBytes</span><span class="sxs-lookup"><span data-stu-id="301b0-134">queueBufferSizeInBytes</span></span>|<span data-ttu-id="301b0-135">Int32</span><span class="sxs-lookup"><span data-stu-id="301b0-135">Int32</span></span>|<span data-ttu-id="301b0-136">O tamanho máximo da fila de trabalho de impressão que pode ser armazenado pela impressora.</span><span class="sxs-lookup"><span data-stu-id="301b0-136">The maximum print job queue size that can be stored by the printer.</span></span>|
|<span data-ttu-id="301b0-137">copiesPerJob</span><span class="sxs-lookup"><span data-stu-id="301b0-137">copiesPerJob</span></span>|[<span data-ttu-id="301b0-138">integerRange</span><span class="sxs-lookup"><span data-stu-id="301b0-138">integerRange</span></span>](integerrange.md)|<span data-ttu-id="301b0-139">O intervalo de cópias por trabalho suportado pela impressora.</span><span class="sxs-lookup"><span data-stu-id="301b0-139">The range of copies per job supported by the printer.</span></span>|
|<span data-ttu-id="301b0-140">finishings</span><span class="sxs-lookup"><span data-stu-id="301b0-140">finishings</span></span>|<span data-ttu-id="301b0-141">[Coleção printFinishing](enums.md#printfinishing-values)</span><span class="sxs-lookup"><span data-stu-id="301b0-141">[printFinishing](enums.md#printfinishing-values) collection</span></span>|<span data-ttu-id="301b0-142">Processos de término que a impressora dá suporte a um documento impresso.</span><span class="sxs-lookup"><span data-stu-id="301b0-142">Finishing processes the printer supports for a printed document.</span></span>|
|<span data-ttu-id="301b0-143">mediaColors</span><span class="sxs-lookup"><span data-stu-id="301b0-143">mediaColors</span></span>|<span data-ttu-id="301b0-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="301b0-144">String collection</span></span>|<span data-ttu-id="301b0-145">As cores de mídia (ou seja, papel) suportadas pela impressora.</span><span class="sxs-lookup"><span data-stu-id="301b0-145">The media (i.e., paper) colors supported by the printer.</span></span>|
|<span data-ttu-id="301b0-146">mediaTypes</span><span class="sxs-lookup"><span data-stu-id="301b0-146">mediaTypes</span></span>|<span data-ttu-id="301b0-147">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="301b0-147">String collection</span></span>|<span data-ttu-id="301b0-148">Os tipos de mídia suportados pela impressora.</span><span class="sxs-lookup"><span data-stu-id="301b0-148">The media types supported by the printer.</span></span> <span data-ttu-id="301b0-149">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="301b0-149">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="301b0-150">mediaSizes</span><span class="sxs-lookup"><span data-stu-id="301b0-150">mediaSizes</span></span>|<span data-ttu-id="301b0-151">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="301b0-151">String collection</span></span>|<span data-ttu-id="301b0-152">Os tamanhos de mídia suportados pela impressora.</span><span class="sxs-lookup"><span data-stu-id="301b0-152">The media sizes supported by the printer.</span></span> <span data-ttu-id="301b0-153">Oferece suporte a nomes de tamanho padrão para tamanhos de mídia ISO e ANSI, juntamente com todos os tamanhos personalizados suportados pela impressora associada.</span><span class="sxs-lookup"><span data-stu-id="301b0-153">Supports standard size names for ISO and ANSI media sizes, along with any custom sizes supported by the associated printer.</span></span>|
|<span data-ttu-id="301b0-154">pagesPerSheet</span><span class="sxs-lookup"><span data-stu-id="301b0-154">pagesPerSheet</span></span>|<span data-ttu-id="301b0-155">Coleção Int32</span><span class="sxs-lookup"><span data-stu-id="301b0-155">Int32 collection</span></span>|<span data-ttu-id="301b0-156">Número suportado de Páginas de Entrada para impor uma única Impressão.</span><span class="sxs-lookup"><span data-stu-id="301b0-156">Supported number of Input Pages to impose upon a single Impression.</span></span>|
|<span data-ttu-id="301b0-157">orientações</span><span class="sxs-lookup"><span data-stu-id="301b0-157">orientations</span></span>|<span data-ttu-id="301b0-158">[Coleção printOrientation](enums.md#printorientation-values)</span><span class="sxs-lookup"><span data-stu-id="301b0-158">[printOrientation](enums.md#printorientation-values) collection</span></span>|<span data-ttu-id="301b0-159">As orientações de impressão suportadas pela impressora.</span><span class="sxs-lookup"><span data-stu-id="301b0-159">The print orientations supported by the printer.</span></span> <span data-ttu-id="301b0-160">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="301b0-160">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="301b0-161">inputBins</span><span class="sxs-lookup"><span data-stu-id="301b0-161">inputBins</span></span>|<span data-ttu-id="301b0-162">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="301b0-162">String collection</span></span>|<span data-ttu-id="301b0-163">Caixas de entrada com suporte para a impressora.</span><span class="sxs-lookup"><span data-stu-id="301b0-163">Supported input bins for the printer.</span></span>|
|<span data-ttu-id="301b0-164">outputBins</span><span class="sxs-lookup"><span data-stu-id="301b0-164">outputBins</span></span>|<span data-ttu-id="301b0-165">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="301b0-165">String collection</span></span>|<span data-ttu-id="301b0-166">As caixas de saída com suporte da impressora (bandejas).</span><span class="sxs-lookup"><span data-stu-id="301b0-166">The printer's supported output bins (trays).</span></span>|
|<span data-ttu-id="301b0-167">supportsFitPdfToPage</span><span class="sxs-lookup"><span data-stu-id="301b0-167">supportsFitPdfToPage</span></span>|<span data-ttu-id="301b0-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="301b0-168">Boolean</span></span>|<span data-ttu-id="301b0-169">True se a impressora oferece suporte ao dimensionamento de páginas PDF para corresponder ao tamanho da mídia de impressão; false caso contrário.</span><span class="sxs-lookup"><span data-stu-id="301b0-169">True if the printer supports scaling PDF pages to match the print media size; false otherwise.</span></span>|
|<span data-ttu-id="301b0-170">multipageLayouts</span><span class="sxs-lookup"><span data-stu-id="301b0-170">multipageLayouts</span></span>|<span data-ttu-id="301b0-171">[Coleção printMultipageLayout](enums.md#printmultipagelayout-values)</span><span class="sxs-lookup"><span data-stu-id="301b0-171">[printMultipageLayout](enums.md#printmultipagelayout-values) collection</span></span>|<span data-ttu-id="301b0-172">As instruções de apresentação suportadas pela impressora.</span><span class="sxs-lookup"><span data-stu-id="301b0-172">The presentation directions supported by the printer.</span></span> <span data-ttu-id="301b0-173">Os valores com suporte são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="301b0-173">Supported values are described in the following table.</span></span>|
|<span data-ttu-id="301b0-174">colorModes</span><span class="sxs-lookup"><span data-stu-id="301b0-174">colorModes</span></span>|<span data-ttu-id="301b0-175">[Coleção printColorMode](enums.md#printcolormode-values)</span><span class="sxs-lookup"><span data-stu-id="301b0-175">[printColorMode](enums.md#printcolormode-values) collection</span></span>|<span data-ttu-id="301b0-176">Os modos de cor suportados pela impressora.</span><span class="sxs-lookup"><span data-stu-id="301b0-176">The color modes supported by the printer.</span></span> <span data-ttu-id="301b0-177">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="301b0-177">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="301b0-178">topMargins</span><span class="sxs-lookup"><span data-stu-id="301b0-178">topMargins</span></span>|<span data-ttu-id="301b0-179">Coleção Int32</span><span class="sxs-lookup"><span data-stu-id="301b0-179">Int32 collection</span></span>|<span data-ttu-id="301b0-180">Uma lista de margens principais com suporte (em mícrons) para a impressora.</span><span class="sxs-lookup"><span data-stu-id="301b0-180">A list of supported top margins(in microns) for the printer.</span></span>|
|<span data-ttu-id="301b0-181">bottomMargins</span><span class="sxs-lookup"><span data-stu-id="301b0-181">bottomMargins</span></span>|<span data-ttu-id="301b0-182">Coleção Int32</span><span class="sxs-lookup"><span data-stu-id="301b0-182">Int32 collection</span></span>|<span data-ttu-id="301b0-183">Uma lista de margens inferior suportadas (em mícrons) para a impressora.</span><span class="sxs-lookup"><span data-stu-id="301b0-183">A list of supported bottom margins(in microns) for the printer.</span></span>|
|<span data-ttu-id="301b0-184">rightMargins</span><span class="sxs-lookup"><span data-stu-id="301b0-184">rightMargins</span></span>|<span data-ttu-id="301b0-185">Coleção Int32</span><span class="sxs-lookup"><span data-stu-id="301b0-185">Int32 collection</span></span>|<span data-ttu-id="301b0-186">Uma lista de margens direitas com suporte (em mícrons) para a impressora.</span><span class="sxs-lookup"><span data-stu-id="301b0-186">A list of supported right margins(in microns) for the printer.</span></span>|
|<span data-ttu-id="301b0-187">leftMargins</span><span class="sxs-lookup"><span data-stu-id="301b0-187">leftMargins</span></span>|<span data-ttu-id="301b0-188">Coleção Int32</span><span class="sxs-lookup"><span data-stu-id="301b0-188">Int32 collection</span></span>|<span data-ttu-id="301b0-189">Uma lista de margens esquerdas suportadas (em mícrons) para a impressora.</span><span class="sxs-lookup"><span data-stu-id="301b0-189">A list of supported left margins(in microns) for the printer.</span></span>|
|<span data-ttu-id="301b0-190">collation</span><span class="sxs-lookup"><span data-stu-id="301b0-190">collation</span></span>|<span data-ttu-id="301b0-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="301b0-191">Boolean</span></span>|<span data-ttu-id="301b0-192">True se a impressora dá suporte à colagem ao imprimir cópias muliplas de um documento de várias páginas; false caso contrário.</span><span class="sxs-lookup"><span data-stu-id="301b0-192">True if the printer supports collating when printing muliple copies of a multi-page document; false otherwise.</span></span>|
|<span data-ttu-id="301b0-193">scalings</span><span class="sxs-lookup"><span data-stu-id="301b0-193">scalings</span></span>|<span data-ttu-id="301b0-194">[Coleção printScaling](enums.md#printscaling-values)</span><span class="sxs-lookup"><span data-stu-id="301b0-194">[printScaling](enums.md#printscaling-values) collection</span></span>|<span data-ttu-id="301b0-195">Dimensionamentos de impressão com suporte.</span><span class="sxs-lookup"><span data-stu-id="301b0-195">Supported print scalings.</span></span>|

## <a name="relationships"></a><span data-ttu-id="301b0-196">Relações</span><span class="sxs-lookup"><span data-stu-id="301b0-196">Relationships</span></span>
<span data-ttu-id="301b0-197">Nenhum</span><span class="sxs-lookup"><span data-stu-id="301b0-197">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="301b0-198">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="301b0-198">JSON representation</span></span>
<span data-ttu-id="301b0-199">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="301b0-199">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printerCapabilities"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerCapabilities",
  "contentTypes": [
    "String"
  ],
  "isColorPrintingSupported": "Boolean",
  "feedOrientations": [
    "String"
  ],
  "isPageRangeSupported": "Boolean",
  "qualities": [
    "String"
  ],
  "dpis": [
    "Integer"
  ],
  "duplexModes": [
    "String"
  ],
  "copiesPerJob": {
    "@odata.type": "microsoft.graph.integerRange"
  },
  "finishings": [
    "String"
  ],
  "mediaColors": [
    "String"
  ],
  "mediaTypes": [
    "String"
  ],
  "mediaSizes": [
    "String"
  ],
  "pagesPerSheet": [
    "Integer"
  ],
  "orientations": [
    "String"
  ],
  "outputBins": [
    "String"
  ],
  "supportsFitPdfToPage": "Boolean",
  "multipageLayouts": [
    "String"
  ],
  "colorModes": [
    "String"
  ],
  "inputBins": [
    "String"
  ],
  "topMargins": [
    "Integer"
  ],
  "bottomMargins": [
    "Integer"
  ],
  "rightMargins": [
    "Integer"
  ],
  "leftMargins": [
    "Integer"
  ],
  "collation": "Boolean",
  "scalings": [
    "String"
  ]
}
```

