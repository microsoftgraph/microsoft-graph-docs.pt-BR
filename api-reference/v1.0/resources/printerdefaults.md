---
title: Tipo de recurso printerDefaults
description: Representa as configurações padrão da impressora. Verifique os recursos da impressora para ver todos os valores compatíveis.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 06566b30e2292d6552e5c0a79281693b97ab6350
ms.sourcegitcommit: 6e7d9987a255f1bee04f196a4a7e37f56621bfb8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2021
ms.locfileid: "51944238"
---
# <a name="printerdefaults-resource-type"></a><span data-ttu-id="a8b35-104">Tipo de recurso printerDefaults</span><span class="sxs-lookup"><span data-stu-id="a8b35-104">printerDefaults resource type</span></span>

<span data-ttu-id="a8b35-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8b35-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="a8b35-106">Representa as configurações padrão da impressora.</span><span class="sxs-lookup"><span data-stu-id="a8b35-106">Represents the printer's default settings.</span></span> <span data-ttu-id="a8b35-107">Verifique os recursos da [impressora para](printercapabilities.md) ver todos os valores compatíveis.</span><span class="sxs-lookup"><span data-stu-id="a8b35-107">Check the printer's [capabilities](printercapabilities.md) to see all the values that it supports.</span></span>

## <a name="properties"></a><span data-ttu-id="a8b35-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a8b35-108">Properties</span></span>
|<span data-ttu-id="a8b35-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8b35-109">Property</span></span>|<span data-ttu-id="a8b35-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8b35-110">Type</span></span>|<span data-ttu-id="a8b35-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8b35-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8b35-112">copiesPerJob</span><span class="sxs-lookup"><span data-stu-id="a8b35-112">copiesPerJob</span></span>|<span data-ttu-id="a8b35-113">Int32</span><span class="sxs-lookup"><span data-stu-id="a8b35-113">Int32</span></span>|<span data-ttu-id="a8b35-114">O número padrão de cópias impressas por trabalho.</span><span class="sxs-lookup"><span data-stu-id="a8b35-114">The default number of copies printed per job.</span></span>|
|<span data-ttu-id="a8b35-115">contentType</span><span class="sxs-lookup"><span data-stu-id="a8b35-115">contentType</span></span>|<span data-ttu-id="a8b35-116">String</span><span class="sxs-lookup"><span data-stu-id="a8b35-116">String</span></span>|<span data-ttu-id="a8b35-117">O tipo de conteúdo padrão (MIME) a ser usado ao processar documentos.</span><span class="sxs-lookup"><span data-stu-id="a8b35-117">The default content (MIME) type to use when processing documents.</span></span>|
|<span data-ttu-id="a8b35-118">finishings</span><span class="sxs-lookup"><span data-stu-id="a8b35-118">finishings</span></span>|<span data-ttu-id="a8b35-119">[Coleção printFinishing](enums.md#printfinishing-values)</span><span class="sxs-lookup"><span data-stu-id="a8b35-119">[printFinishing](enums.md#printfinishing-values) collection</span></span>|<span data-ttu-id="a8b35-120">O conjunto padrão de acabamentos a ser aplicado a trabalhos de impressão.</span><span class="sxs-lookup"><span data-stu-id="a8b35-120">The default set of finishings to apply to print jobs.</span></span> <span data-ttu-id="a8b35-121">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="a8b35-121">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="a8b35-122">mediaColor</span><span class="sxs-lookup"><span data-stu-id="a8b35-122">mediaColor</span></span>|<span data-ttu-id="a8b35-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8b35-123">String</span></span>|<span data-ttu-id="a8b35-124">A cor padrão da mídia (como papel) para imprimir o documento.</span><span class="sxs-lookup"><span data-stu-id="a8b35-124">The default media (such as paper) color to print the document on.</span></span>|
|<span data-ttu-id="a8b35-125">mediaType</span><span class="sxs-lookup"><span data-stu-id="a8b35-125">mediaType</span></span>|<span data-ttu-id="a8b35-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8b35-126">String</span></span>|<span data-ttu-id="a8b35-127">O tipo de mídia padrão (como papel) para imprimir o documento.</span><span class="sxs-lookup"><span data-stu-id="a8b35-127">The default media (such as paper) type to print the document on.</span></span>|
|<span data-ttu-id="a8b35-128">mediaSize</span><span class="sxs-lookup"><span data-stu-id="a8b35-128">mediaSize</span></span>|<span data-ttu-id="a8b35-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8b35-129">String</span></span>|<span data-ttu-id="a8b35-130">O tamanho de mídia padrão a ser usado.</span><span class="sxs-lookup"><span data-stu-id="a8b35-130">The default media size to use.</span></span> <span data-ttu-id="a8b35-131">Oferece suporte a nomes de tamanho padrão para tamanhos de mídia ISO e ANSI.</span><span class="sxs-lookup"><span data-stu-id="a8b35-131">Supports standard size names for ISO and ANSI media sizes.</span></span> <span data-ttu-id="a8b35-132">Os valores válidos são listados no tópico [printerCapabilities.](printercapabilities.md#mediasizes-values)</span><span class="sxs-lookup"><span data-stu-id="a8b35-132">Valid values are listed in the [printerCapabilities](printercapabilities.md#mediasizes-values) topic.</span></span>|
|<span data-ttu-id="a8b35-133">pagesPerSheet</span><span class="sxs-lookup"><span data-stu-id="a8b35-133">pagesPerSheet</span></span>|<span data-ttu-id="a8b35-134">Int32</span><span class="sxs-lookup"><span data-stu-id="a8b35-134">Int32</span></span>|<span data-ttu-id="a8b35-135">O número padrão de páginas de documento a ser impressa em cada planilha.</span><span class="sxs-lookup"><span data-stu-id="a8b35-135">The default number of document pages to print on each sheet.</span></span>
|<span data-ttu-id="a8b35-136">orientation</span><span class="sxs-lookup"><span data-stu-id="a8b35-136">orientation</span></span>|[<span data-ttu-id="a8b35-137">printOrientation</span><span class="sxs-lookup"><span data-stu-id="a8b35-137">printOrientation</span></span>](enums.md#printorientation-values)|<span data-ttu-id="a8b35-138">A orientação padrão a ser usada ao imprimir o documento.</span><span class="sxs-lookup"><span data-stu-id="a8b35-138">The default orientation to use when printing the document.</span></span> <span data-ttu-id="a8b35-139">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="a8b35-139">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="a8b35-140">outputBin</span><span class="sxs-lookup"><span data-stu-id="a8b35-140">outputBin</span></span>|<span data-ttu-id="a8b35-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8b35-141">String</span></span>|<span data-ttu-id="a8b35-142">A lixeira de saída padrão para colocar as impressões concluídas.</span><span class="sxs-lookup"><span data-stu-id="a8b35-142">The default output bin to place completed prints into.</span></span> <span data-ttu-id="a8b35-143">Consulte os recursos da [impressora para](printercapabilities.md) uma lista de caixas de saída com suporte.</span><span class="sxs-lookup"><span data-stu-id="a8b35-143">See the printer's [capabilities](printercapabilities.md) for a list of supported output bins.</span></span>|
|<span data-ttu-id="a8b35-144">fitPdfToPage</span><span class="sxs-lookup"><span data-stu-id="a8b35-144">fitPdfToPage</span></span>|<span data-ttu-id="a8b35-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="a8b35-145">Boolean</span></span>|<span data-ttu-id="a8b35-146">A configuração padrão fitPdfToPage.</span><span class="sxs-lookup"><span data-stu-id="a8b35-146">The default fitPdfToPage setting.</span></span> <span data-ttu-id="a8b35-147">True para ajustar cada página de um documento PDF a uma folha física de mídia; false para permitir que a impressora decida como definir impressões.</span><span class="sxs-lookup"><span data-stu-id="a8b35-147">True to fit each page of a PDF document to a physical sheet of media; false to let the printer decide how to lay out impressions.</span></span>|
|<span data-ttu-id="a8b35-148">multipageLayout</span><span class="sxs-lookup"><span data-stu-id="a8b35-148">multipageLayout</span></span>|[<span data-ttu-id="a8b35-149">printMultipageLayout</span><span class="sxs-lookup"><span data-stu-id="a8b35-149">printMultipageLayout</span></span>](enums.md#printmultipagelayout-values)|<span data-ttu-id="a8b35-150">A direção padrão para colocar as páginas quando várias páginas estão sendo impressas por planilha.</span><span class="sxs-lookup"><span data-stu-id="a8b35-150">The default direction to lay out pages when multiple pages are being printed per sheet.</span></span> <span data-ttu-id="a8b35-151">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="a8b35-151">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="a8b35-152">colorMode</span><span class="sxs-lookup"><span data-stu-id="a8b35-152">colorMode</span></span>|[<span data-ttu-id="a8b35-153">printColorMode</span><span class="sxs-lookup"><span data-stu-id="a8b35-153">printColorMode</span></span>](enums.md#printcolormode-values)|<span data-ttu-id="a8b35-154">O modo de cor padrão a ser usado ao imprimir o documento.</span><span class="sxs-lookup"><span data-stu-id="a8b35-154">The default color mode to use when printing the document.</span></span> <span data-ttu-id="a8b35-155">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="a8b35-155">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="a8b35-156">quality</span><span class="sxs-lookup"><span data-stu-id="a8b35-156">quality</span></span>|[<span data-ttu-id="a8b35-157">printQuality</span><span class="sxs-lookup"><span data-stu-id="a8b35-157">printQuality</span></span>](enums.md#printquality-values)|<span data-ttu-id="a8b35-158">A qualidade padrão a ser usada ao imprimir o documento.</span><span class="sxs-lookup"><span data-stu-id="a8b35-158">The default quality to use when printing the document.</span></span> <span data-ttu-id="a8b35-159">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="a8b35-159">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="a8b35-160">duplexMode</span><span class="sxs-lookup"><span data-stu-id="a8b35-160">duplexMode</span></span>|[<span data-ttu-id="a8b35-161">printDuplexMode</span><span class="sxs-lookup"><span data-stu-id="a8b35-161">printDuplexMode</span></span>](enums.md#printduplexmode-values)|<span data-ttu-id="a8b35-162">A configuração duplex padrão (com duas laterais) a ser usada ao imprimir um documento.</span><span class="sxs-lookup"><span data-stu-id="a8b35-162">The default duplex (double-sided) configuration to use when printing a document.</span></span> <span data-ttu-id="a8b35-163">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="a8b35-163">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="a8b35-164">dpi</span><span class="sxs-lookup"><span data-stu-id="a8b35-164">dpi</span></span>|<span data-ttu-id="a8b35-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a8b35-165">Int32</span></span>|<span data-ttu-id="a8b35-166">A resolução padrão no DPI a ser usada ao imprimir o trabalho.</span><span class="sxs-lookup"><span data-stu-id="a8b35-166">The default resolution in DPI to use when printing the job.</span></span>|
|<span data-ttu-id="a8b35-167">scaling</span><span class="sxs-lookup"><span data-stu-id="a8b35-167">scaling</span></span>|[<span data-ttu-id="a8b35-168">printScaling</span><span class="sxs-lookup"><span data-stu-id="a8b35-168">printScaling</span></span>](enums.md#printscaling-values)|<span data-ttu-id="a8b35-169">Especifica como a impressora dimensiona os dados do documento para se ajustar à mídia solicitada.</span><span class="sxs-lookup"><span data-stu-id="a8b35-169">Specifies how the printer scales the document data to fit the requested media.</span></span> <span data-ttu-id="a8b35-170">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="a8b35-170">Valid values are described in the following table.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8b35-171">Relações</span><span class="sxs-lookup"><span data-stu-id="a8b35-171">Relationships</span></span>
<span data-ttu-id="a8b35-172">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a8b35-172">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8b35-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a8b35-173">JSON representation</span></span>
<span data-ttu-id="a8b35-174">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a8b35-174">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printerDefaults"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerDefaults",
  "copiesPerJob": "Integer",
  "contentType": "String",
  "finishings": [
    "String"
  ],
  "mediaColor": "String",
  "mediaType": "String",
  "mediaSize": "String",
  "pagesPerSheet": "Integer",
  "orientation": "String",
  "outputBin": "String",
  "inputBin": "String",
  "fitPdfToPage": "Boolean",
  "multipageLayout": "String",
  "colorMode": "String",
  "quality": "String",
  "duplexMode": "String",
  "dpi": "Integer",
  "scaling": "String"
}
```

