---
title: Tipo complexo printerCapabilities
description: Representa os recursos relatados por uma impressora.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: bda913275aff692df2f66472f61436665cbc3dd7
ms.sourcegitcommit: 6e7d9987a255f1bee04f196a4a7e37f56621bfb8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2021
ms.locfileid: "51944223"
---
# <a name="printercapabilities-resource-type"></a><span data-ttu-id="05af9-103">Tipo de recurso printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="05af9-103">printerCapabilities resource type</span></span>

<span data-ttu-id="05af9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05af9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="05af9-105">Representa os recursos relatados por um printer/printerShare.</span><span class="sxs-lookup"><span data-stu-id="05af9-105">Represents the capabilities reported by a printer/printerShare.</span></span>

## <a name="properties"></a><span data-ttu-id="05af9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="05af9-106">Properties</span></span>
| <span data-ttu-id="05af9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05af9-107">Property</span></span>     | <span data-ttu-id="05af9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="05af9-108">Type</span></span>        | <span data-ttu-id="05af9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="05af9-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="05af9-110">contentTypes</span><span class="sxs-lookup"><span data-stu-id="05af9-110">contentTypes</span></span>|<span data-ttu-id="05af9-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="05af9-111">String collection</span></span>|<span data-ttu-id="05af9-112">Uma lista de tipos de conteúdo com suporte (MIME) compatíveis com a impressora.</span><span class="sxs-lookup"><span data-stu-id="05af9-112">A list of supported content (MIME) types that the printer supports.</span></span> <span data-ttu-id="05af9-113">Não é garantido que o serviço Impressão Universal dá suporte à impressão de todos esses tipos mime.</span><span class="sxs-lookup"><span data-stu-id="05af9-113">It is not guaranteed that the Universal Print service supports printing all of these MIME types.</span></span>|
|<span data-ttu-id="05af9-114">isColorPrintingSupported</span><span class="sxs-lookup"><span data-stu-id="05af9-114">isColorPrintingSupported</span></span>|<span data-ttu-id="05af9-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="05af9-115">Boolean</span></span>|<span data-ttu-id="05af9-116">True se a impressão de cores for suportada pela impressora; false caso contrário.</span><span class="sxs-lookup"><span data-stu-id="05af9-116">True if color printing is supported by the printer; false otherwise.</span></span> <span data-ttu-id="05af9-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05af9-117">Read-only.</span></span>|
|<span data-ttu-id="05af9-118">feedOrientations</span><span class="sxs-lookup"><span data-stu-id="05af9-118">feedOrientations</span></span>|<span data-ttu-id="05af9-119">Coleção printerFeedOrientation</span><span class="sxs-lookup"><span data-stu-id="05af9-119">printerFeedOrientation collection</span></span>|<span data-ttu-id="05af9-120">A lista de orientações de feed que são suportadas pela impressora.</span><span class="sxs-lookup"><span data-stu-id="05af9-120">The list of feed orientations that are supported by the printer.</span></span>|
|<span data-ttu-id="05af9-121">isPageRangeSupported</span><span class="sxs-lookup"><span data-stu-id="05af9-121">isPageRangeSupported</span></span>|<span data-ttu-id="05af9-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="05af9-122">Boolean</span></span>|<span data-ttu-id="05af9-123">True se a impressora dá suporte à impressão por intervalos de página; false caso contrário.</span><span class="sxs-lookup"><span data-stu-id="05af9-123">True if the printer supports printing by page ranges; false otherwise.</span></span>|
|<span data-ttu-id="05af9-124">qualidades</span><span class="sxs-lookup"><span data-stu-id="05af9-124">qualities</span></span>|<span data-ttu-id="05af9-125">[Coleção printQuality](enums.md#printquality-values)</span><span class="sxs-lookup"><span data-stu-id="05af9-125">[printQuality](enums.md#printquality-values) collection</span></span>|<span data-ttu-id="05af9-126">As qualidades de impressão suportadas pela impressora.</span><span class="sxs-lookup"><span data-stu-id="05af9-126">The print qualities supported by the printer.</span></span>|
|<span data-ttu-id="05af9-127">dpis</span><span class="sxs-lookup"><span data-stu-id="05af9-127">dpis</span></span>|<span data-ttu-id="05af9-128">Coleção Int32</span><span class="sxs-lookup"><span data-stu-id="05af9-128">Int32 collection</span></span>|<span data-ttu-id="05af9-129">A lista de resoluções de impressão em DPI que são suportadas pela impressora.</span><span class="sxs-lookup"><span data-stu-id="05af9-129">The list of print resolutions in DPI that are supported by the printer.</span></span>|
|<span data-ttu-id="05af9-130">duplexModes</span><span class="sxs-lookup"><span data-stu-id="05af9-130">duplexModes</span></span>|<span data-ttu-id="05af9-131">[Coleção printDuplexMode](enums.md#printduplexmode-values)</span><span class="sxs-lookup"><span data-stu-id="05af9-131">[printDuplexMode](enums.md#printduplexmode-values) collection</span></span>|<span data-ttu-id="05af9-132">A lista de modos duplex com suporte da impressora.</span><span class="sxs-lookup"><span data-stu-id="05af9-132">The list of duplex modes that are supported by the printer.</span></span> <span data-ttu-id="05af9-133">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="05af9-133">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="05af9-134">queueBufferSizeInBytes</span><span class="sxs-lookup"><span data-stu-id="05af9-134">queueBufferSizeInBytes</span></span>|<span data-ttu-id="05af9-135">Int32</span><span class="sxs-lookup"><span data-stu-id="05af9-135">Int32</span></span>|<span data-ttu-id="05af9-136">O tamanho máximo da fila de trabalho de impressão que pode ser armazenado pela impressora.</span><span class="sxs-lookup"><span data-stu-id="05af9-136">The maximum print job queue size that can be stored by the printer.</span></span>|
|<span data-ttu-id="05af9-137">copiesPerJob</span><span class="sxs-lookup"><span data-stu-id="05af9-137">copiesPerJob</span></span>|[<span data-ttu-id="05af9-138">integerRange</span><span class="sxs-lookup"><span data-stu-id="05af9-138">integerRange</span></span>](integerrange.md)|<span data-ttu-id="05af9-139">O intervalo de cópias por trabalho suportado pela impressora.</span><span class="sxs-lookup"><span data-stu-id="05af9-139">The range of copies per job supported by the printer.</span></span>|
|<span data-ttu-id="05af9-140">finishings</span><span class="sxs-lookup"><span data-stu-id="05af9-140">finishings</span></span>|<span data-ttu-id="05af9-141">[Coleção printFinishing](enums.md#printfinishing-values)</span><span class="sxs-lookup"><span data-stu-id="05af9-141">[printFinishing](enums.md#printfinishing-values) collection</span></span>|<span data-ttu-id="05af9-142">Processos de término que a impressora dá suporte a um documento impresso.</span><span class="sxs-lookup"><span data-stu-id="05af9-142">Finishing processes the printer supports for a printed document.</span></span>|
|<span data-ttu-id="05af9-143">mediaColors</span><span class="sxs-lookup"><span data-stu-id="05af9-143">mediaColors</span></span>|<span data-ttu-id="05af9-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="05af9-144">String collection</span></span>|<span data-ttu-id="05af9-145">As cores de mídia (ou seja, papel) suportadas pela impressora.</span><span class="sxs-lookup"><span data-stu-id="05af9-145">The media (i.e., paper) colors supported by the printer.</span></span>|
|<span data-ttu-id="05af9-146">mediaTypes</span><span class="sxs-lookup"><span data-stu-id="05af9-146">mediaTypes</span></span>|<span data-ttu-id="05af9-147">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="05af9-147">String collection</span></span>|<span data-ttu-id="05af9-148">Os tipos de mídia suportados pela impressora.</span><span class="sxs-lookup"><span data-stu-id="05af9-148">The media types supported by the printer.</span></span>|
|<span data-ttu-id="05af9-149">mediaSizes</span><span class="sxs-lookup"><span data-stu-id="05af9-149">mediaSizes</span></span>|<span data-ttu-id="05af9-150">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="05af9-150">String collection</span></span>|<span data-ttu-id="05af9-151">Os tamanhos de mídia suportados pela impressora.</span><span class="sxs-lookup"><span data-stu-id="05af9-151">The media sizes supported by the printer.</span></span> <span data-ttu-id="05af9-152">Oferece suporte a nomes de tamanho padrão para tamanhos de mídia ISO e ANSI.</span><span class="sxs-lookup"><span data-stu-id="05af9-152">Supports standard size names for ISO and ANSI media sizes.</span></span> <span data-ttu-id="05af9-153">Os valores válidos estão na tabela [a seguir](#mediasizes-values).</span><span class="sxs-lookup"><span data-stu-id="05af9-153">Valid values are in the following [table](#mediasizes-values).</span></span>|
|<span data-ttu-id="05af9-154">pagesPerSheet</span><span class="sxs-lookup"><span data-stu-id="05af9-154">pagesPerSheet</span></span>|<span data-ttu-id="05af9-155">Coleção Int32</span><span class="sxs-lookup"><span data-stu-id="05af9-155">Int32 collection</span></span>|<span data-ttu-id="05af9-156">Número suportado de Páginas de Entrada para impor uma única Impressão.</span><span class="sxs-lookup"><span data-stu-id="05af9-156">Supported number of Input Pages to impose upon a single Impression.</span></span>|
|<span data-ttu-id="05af9-157">orientações</span><span class="sxs-lookup"><span data-stu-id="05af9-157">orientations</span></span>|<span data-ttu-id="05af9-158">[Coleção printOrientation](enums.md#printorientation-values)</span><span class="sxs-lookup"><span data-stu-id="05af9-158">[printOrientation](enums.md#printorientation-values) collection</span></span>|<span data-ttu-id="05af9-159">As orientações de impressão suportadas pela impressora.</span><span class="sxs-lookup"><span data-stu-id="05af9-159">The print orientations supported by the printer.</span></span> <span data-ttu-id="05af9-160">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="05af9-160">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="05af9-161">inputBins</span><span class="sxs-lookup"><span data-stu-id="05af9-161">inputBins</span></span>|<span data-ttu-id="05af9-162">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="05af9-162">String collection</span></span>|<span data-ttu-id="05af9-163">Caixas de entrada com suporte para a impressora.</span><span class="sxs-lookup"><span data-stu-id="05af9-163">Supported input bins for the printer.</span></span>|
|<span data-ttu-id="05af9-164">outputBins</span><span class="sxs-lookup"><span data-stu-id="05af9-164">outputBins</span></span>|<span data-ttu-id="05af9-165">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="05af9-165">String collection</span></span>|<span data-ttu-id="05af9-166">As caixas de saída com suporte da impressora (bandejas).</span><span class="sxs-lookup"><span data-stu-id="05af9-166">The printer's supported output bins (trays).</span></span>|
|<span data-ttu-id="05af9-167">supportsFitPdfToPage</span><span class="sxs-lookup"><span data-stu-id="05af9-167">supportsFitPdfToPage</span></span>|<span data-ttu-id="05af9-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="05af9-168">Boolean</span></span>|<span data-ttu-id="05af9-169">True se a impressora oferece suporte ao dimensionamento de páginas PDF para corresponder ao tamanho da mídia de impressão; false caso contrário.</span><span class="sxs-lookup"><span data-stu-id="05af9-169">True if the printer supports scaling PDF pages to match the print media size; false otherwise.</span></span>|
|<span data-ttu-id="05af9-170">multipageLayouts</span><span class="sxs-lookup"><span data-stu-id="05af9-170">multipageLayouts</span></span>|<span data-ttu-id="05af9-171">[Coleção printMultipageLayout](enums.md#printmultipagelayout-values)</span><span class="sxs-lookup"><span data-stu-id="05af9-171">[printMultipageLayout](enums.md#printmultipagelayout-values) collection</span></span>|<span data-ttu-id="05af9-172">As instruções de apresentação suportadas pela impressora.</span><span class="sxs-lookup"><span data-stu-id="05af9-172">The presentation directions supported by the printer.</span></span> <span data-ttu-id="05af9-173">Os valores com suporte são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="05af9-173">Supported values are described in the following table.</span></span>|
|<span data-ttu-id="05af9-174">colorModes</span><span class="sxs-lookup"><span data-stu-id="05af9-174">colorModes</span></span>|<span data-ttu-id="05af9-175">[Coleção printColorMode](enums.md#printcolormode-values)</span><span class="sxs-lookup"><span data-stu-id="05af9-175">[printColorMode](enums.md#printcolormode-values) collection</span></span>|<span data-ttu-id="05af9-176">Os modos de cor suportados pela impressora.</span><span class="sxs-lookup"><span data-stu-id="05af9-176">The color modes supported by the printer.</span></span> <span data-ttu-id="05af9-177">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="05af9-177">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="05af9-178">topMargins</span><span class="sxs-lookup"><span data-stu-id="05af9-178">topMargins</span></span>|<span data-ttu-id="05af9-179">Coleção Int32</span><span class="sxs-lookup"><span data-stu-id="05af9-179">Int32 collection</span></span>|<span data-ttu-id="05af9-180">Uma lista de margens principais com suporte (em mícrons) para a impressora.</span><span class="sxs-lookup"><span data-stu-id="05af9-180">A list of supported top margins(in microns) for the printer.</span></span>|
|<span data-ttu-id="05af9-181">bottomMargins</span><span class="sxs-lookup"><span data-stu-id="05af9-181">bottomMargins</span></span>|<span data-ttu-id="05af9-182">Coleção Int32</span><span class="sxs-lookup"><span data-stu-id="05af9-182">Int32 collection</span></span>|<span data-ttu-id="05af9-183">Uma lista de margens inferior suportadas (em mícrons) para a impressora.</span><span class="sxs-lookup"><span data-stu-id="05af9-183">A list of supported bottom margins(in microns) for the printer.</span></span>|
|<span data-ttu-id="05af9-184">rightMargins</span><span class="sxs-lookup"><span data-stu-id="05af9-184">rightMargins</span></span>|<span data-ttu-id="05af9-185">Coleção Int32</span><span class="sxs-lookup"><span data-stu-id="05af9-185">Int32 collection</span></span>|<span data-ttu-id="05af9-186">Uma lista de margens direitas com suporte (em mícrons) para a impressora.</span><span class="sxs-lookup"><span data-stu-id="05af9-186">A list of supported right margins(in microns) for the printer.</span></span>|
|<span data-ttu-id="05af9-187">leftMargins</span><span class="sxs-lookup"><span data-stu-id="05af9-187">leftMargins</span></span>|<span data-ttu-id="05af9-188">Coleção Int32</span><span class="sxs-lookup"><span data-stu-id="05af9-188">Int32 collection</span></span>|<span data-ttu-id="05af9-189">Uma lista de margens esquerdas suportadas (em mícrons) para a impressora.</span><span class="sxs-lookup"><span data-stu-id="05af9-189">A list of supported left margins(in microns) for the printer.</span></span>|
|<span data-ttu-id="05af9-190">collation</span><span class="sxs-lookup"><span data-stu-id="05af9-190">collation</span></span>|<span data-ttu-id="05af9-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="05af9-191">Boolean</span></span>|<span data-ttu-id="05af9-192">True se a impressora dá suporte à colagem ao imprimir cópias muliplas de um documento de várias páginas; false caso contrário.</span><span class="sxs-lookup"><span data-stu-id="05af9-192">True if the printer supports collating when printing muliple copies of a multi-page document; false otherwise.</span></span>|
|<span data-ttu-id="05af9-193">scalings</span><span class="sxs-lookup"><span data-stu-id="05af9-193">scalings</span></span>|<span data-ttu-id="05af9-194">[Coleção printScaling](enums.md#printscaling-values)</span><span class="sxs-lookup"><span data-stu-id="05af9-194">[printScaling](enums.md#printscaling-values) collection</span></span>|<span data-ttu-id="05af9-195">Dimensionamentos de impressão com suporte.</span><span class="sxs-lookup"><span data-stu-id="05af9-195">Supported print scalings.</span></span>|

### <a name="mediasizes-values"></a><span data-ttu-id="05af9-196">mediaSizes values</span><span class="sxs-lookup"><span data-stu-id="05af9-196">mediaSizes values</span></span>

|<span data-ttu-id="05af9-197">Valor</span><span class="sxs-lookup"><span data-stu-id="05af9-197">Value</span></span>|
|:---|
|<span data-ttu-id="05af9-198">A3</span><span class="sxs-lookup"><span data-stu-id="05af9-198">A3</span></span>|
|<span data-ttu-id="05af9-199">A4</span><span class="sxs-lookup"><span data-stu-id="05af9-199">A4</span></span>|
|<span data-ttu-id="05af9-200">A5</span><span class="sxs-lookup"><span data-stu-id="05af9-200">A5</span></span>|
|<span data-ttu-id="05af9-201">A6</span><span class="sxs-lookup"><span data-stu-id="05af9-201">A6</span></span>|
|<span data-ttu-id="05af9-202">JIS B4</span><span class="sxs-lookup"><span data-stu-id="05af9-202">JIS B4</span></span>|
|<span data-ttu-id="05af9-203">JIS B5</span><span class="sxs-lookup"><span data-stu-id="05af9-203">JIS B5</span></span>|
|<span data-ttu-id="05af9-204">JPN Hagaki</span><span class="sxs-lookup"><span data-stu-id="05af9-204">JPN Hagaki</span></span>|
|<span data-ttu-id="05af9-205">América do Norte 5x7in</span><span class="sxs-lookup"><span data-stu-id="05af9-205">North America 5x7in</span></span>|
|<span data-ttu-id="05af9-206">Executivo da América do Norte</span><span class="sxs-lookup"><span data-stu-id="05af9-206">North America Executive</span></span>|
|<span data-ttu-id="05af9-207">Carta de Goverment da América do Norte</span><span class="sxs-lookup"><span data-stu-id="05af9-207">North America Goverment Letter</span></span>|
|<span data-ttu-id="05af9-208">Índice da América do Norte 3x5in</span><span class="sxs-lookup"><span data-stu-id="05af9-208">North America Index 3x5in</span></span>|
|<span data-ttu-id="05af9-209">Índice da América do Norte 4x8in</span><span class="sxs-lookup"><span data-stu-id="05af9-209">North America Index 4x8in</span></span>|
|<span data-ttu-id="05af9-210">Índice da América do Norte 5x8in</span><span class="sxs-lookup"><span data-stu-id="05af9-210">North America Index 5x8in</span></span>|
|<span data-ttu-id="05af9-211">Fatura da América do Norte</span><span class="sxs-lookup"><span data-stu-id="05af9-211">North America Invoice</span></span>|
|<span data-ttu-id="05af9-212">Ledger da América do Norte</span><span class="sxs-lookup"><span data-stu-id="05af9-212">North America Ledger</span></span>|
|<span data-ttu-id="05af9-213">América do Norte Legal</span><span class="sxs-lookup"><span data-stu-id="05af9-213">North America Legal</span></span>|
|<span data-ttu-id="05af9-214">Carta da América do Norte</span><span class="sxs-lookup"><span data-stu-id="05af9-214">North America Letter</span></span>|
|<span data-ttu-id="05af9-215">Foto l 3.5x5in</span><span class="sxs-lookup"><span data-stu-id="05af9-215">Photo l 3.5x5in</span></span>|
|<span data-ttu-id="05af9-216">Cartão de Visita</span><span class="sxs-lookup"><span data-stu-id="05af9-216">Business Card</span></span>|
|<span data-ttu-id="05af9-217">Photo</span><span class="sxs-lookup"><span data-stu-id="05af9-217">Photo</span></span>|

## <a name="relationships"></a><span data-ttu-id="05af9-218">Relações</span><span class="sxs-lookup"><span data-stu-id="05af9-218">Relationships</span></span>
<span data-ttu-id="05af9-219">Nenhum</span><span class="sxs-lookup"><span data-stu-id="05af9-219">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="05af9-220">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="05af9-220">JSON representation</span></span>
<span data-ttu-id="05af9-221">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="05af9-221">The following is a JSON representation of the resource.</span></span>
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

