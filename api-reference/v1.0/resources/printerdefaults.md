---
title: Tipo de recurso printerDefaults
description: Representa as configurações padrão da impressora. Verifique os recursos da impressora para ver todos os valores compatíveis.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: fbee453d42fbcb056ce3dce3ff7311e4d976b7dc
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516823"
---
# <a name="printerdefaults-resource-type"></a><span data-ttu-id="84e6e-104">Tipo de recurso printerDefaults</span><span class="sxs-lookup"><span data-stu-id="84e6e-104">printerDefaults resource type</span></span>

<span data-ttu-id="84e6e-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84e6e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="84e6e-106">Representa as configurações padrão da impressora.</span><span class="sxs-lookup"><span data-stu-id="84e6e-106">Represents the printer's default settings.</span></span> <span data-ttu-id="84e6e-107">Verifique os recursos da [impressora para](printercapabilities.md) ver todos os valores compatíveis.</span><span class="sxs-lookup"><span data-stu-id="84e6e-107">Check the printer's [capabilities](printercapabilities.md) to see all the values that it supports.</span></span>

## <a name="properties"></a><span data-ttu-id="84e6e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="84e6e-108">Properties</span></span>
|<span data-ttu-id="84e6e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84e6e-109">Property</span></span>|<span data-ttu-id="84e6e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="84e6e-110">Type</span></span>|<span data-ttu-id="84e6e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="84e6e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84e6e-112">copiesPerJob</span><span class="sxs-lookup"><span data-stu-id="84e6e-112">copiesPerJob</span></span>|<span data-ttu-id="84e6e-113">Int32</span><span class="sxs-lookup"><span data-stu-id="84e6e-113">Int32</span></span>|<span data-ttu-id="84e6e-114">O número padrão de cópias impressas por trabalho.</span><span class="sxs-lookup"><span data-stu-id="84e6e-114">The default number of copies printed per job.</span></span>|
|<span data-ttu-id="84e6e-115">contentType</span><span class="sxs-lookup"><span data-stu-id="84e6e-115">contentType</span></span>|<span data-ttu-id="84e6e-116">String</span><span class="sxs-lookup"><span data-stu-id="84e6e-116">String</span></span>|<span data-ttu-id="84e6e-117">O tipo de conteúdo padrão (MIME) a ser usado ao processar documentos.</span><span class="sxs-lookup"><span data-stu-id="84e6e-117">The default content (MIME) type to use when processing documents.</span></span>|
|<span data-ttu-id="84e6e-118">finishings</span><span class="sxs-lookup"><span data-stu-id="84e6e-118">finishings</span></span>|<span data-ttu-id="84e6e-119">[Coleção printFinishing](enums.md#printfinishing-values)</span><span class="sxs-lookup"><span data-stu-id="84e6e-119">[printFinishing](enums.md#printfinishing-values) collection</span></span>|<span data-ttu-id="84e6e-120">O conjunto padrão de acabamentos a ser aplicado a trabalhos de impressão.</span><span class="sxs-lookup"><span data-stu-id="84e6e-120">The default set of finishings to apply to print jobs.</span></span> <span data-ttu-id="84e6e-121">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="84e6e-121">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="84e6e-122">mediaColor</span><span class="sxs-lookup"><span data-stu-id="84e6e-122">mediaColor</span></span>|<span data-ttu-id="84e6e-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84e6e-123">String</span></span>|<span data-ttu-id="84e6e-124">A cor padrão da mídia (como papel) para imprimir o documento.</span><span class="sxs-lookup"><span data-stu-id="84e6e-124">The default media (such as paper) color to print the document on.</span></span>
|<span data-ttu-id="84e6e-125">mediaType</span><span class="sxs-lookup"><span data-stu-id="84e6e-125">mediaType</span></span>|<span data-ttu-id="84e6e-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84e6e-126">String</span></span>|<span data-ttu-id="84e6e-127">O tipo de mídia padrão (como papel) para imprimir o documento.</span><span class="sxs-lookup"><span data-stu-id="84e6e-127">The default media (such as paper) type to print the document on.</span></span> <span data-ttu-id="84e6e-128">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="84e6e-128">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="84e6e-129">mediaSize</span><span class="sxs-lookup"><span data-stu-id="84e6e-129">mediaSize</span></span>|<span data-ttu-id="84e6e-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84e6e-130">String</span></span>|<span data-ttu-id="84e6e-131">O tamanho de mídia padrão a ser usado.</span><span class="sxs-lookup"><span data-stu-id="84e6e-131">The default media size to use.</span></span> <span data-ttu-id="84e6e-132">Oferece suporte a nomes de tamanho padrão para tamanhos de mídia ISO e ANSI, juntamente com todos os tamanhos personalizados suportados pela impressora associada.</span><span class="sxs-lookup"><span data-stu-id="84e6e-132">Supports standard size names for ISO and ANSI media sizes, along with any custom sizes supported by the associated printer.</span></span>
|<span data-ttu-id="84e6e-133">pagesPerSheet</span><span class="sxs-lookup"><span data-stu-id="84e6e-133">pagesPerSheet</span></span>|<span data-ttu-id="84e6e-134">Int32</span><span class="sxs-lookup"><span data-stu-id="84e6e-134">Int32</span></span>|<span data-ttu-id="84e6e-135">O número padrão de páginas de documento a ser impressa em cada planilha.</span><span class="sxs-lookup"><span data-stu-id="84e6e-135">The default number of document pages to print on each sheet.</span></span>
|<span data-ttu-id="84e6e-136">orientation</span><span class="sxs-lookup"><span data-stu-id="84e6e-136">orientation</span></span>|[<span data-ttu-id="84e6e-137">printOrientation</span><span class="sxs-lookup"><span data-stu-id="84e6e-137">printOrientation</span></span>](enums.md#printorientation-values)|<span data-ttu-id="84e6e-138">A orientação padrão a ser usada ao imprimir o documento.</span><span class="sxs-lookup"><span data-stu-id="84e6e-138">The default orientation to use when printing the document.</span></span> <span data-ttu-id="84e6e-139">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="84e6e-139">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="84e6e-140">outputBin</span><span class="sxs-lookup"><span data-stu-id="84e6e-140">outputBin</span></span>|<span data-ttu-id="84e6e-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84e6e-141">String</span></span>|<span data-ttu-id="84e6e-142">A lixeira de saída padrão para colocar as impressões concluídas.</span><span class="sxs-lookup"><span data-stu-id="84e6e-142">The default output bin to place completed prints into.</span></span> <span data-ttu-id="84e6e-143">Consulte os recursos da [impressora para](printercapabilities.md) uma lista de caixas de saída com suporte.</span><span class="sxs-lookup"><span data-stu-id="84e6e-143">See the printer's [capabilities](printercapabilities.md) for a list of supported output bins.</span></span>|
|<span data-ttu-id="84e6e-144">fitPdfToPage</span><span class="sxs-lookup"><span data-stu-id="84e6e-144">fitPdfToPage</span></span>|<span data-ttu-id="84e6e-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="84e6e-145">Boolean</span></span>|<span data-ttu-id="84e6e-146">A configuração padrão fitPdfToPage.</span><span class="sxs-lookup"><span data-stu-id="84e6e-146">The default fitPdfToPage setting.</span></span> <span data-ttu-id="84e6e-147">True para ajustar cada página de um documento PDF a uma folha física de mídia; false para permitir que a impressora decida como definir impressões.</span><span class="sxs-lookup"><span data-stu-id="84e6e-147">True to fit each page of a PDF document to a physical sheet of media; false to let the printer decide how to lay out impressions.</span></span>|
|<span data-ttu-id="84e6e-148">multipageLayout</span><span class="sxs-lookup"><span data-stu-id="84e6e-148">multipageLayout</span></span>|[<span data-ttu-id="84e6e-149">printMultipageLayout</span><span class="sxs-lookup"><span data-stu-id="84e6e-149">printMultipageLayout</span></span>](enums.md#printmultipagelayout-values)|<span data-ttu-id="84e6e-150">A direção padrão para colocar as páginas quando várias páginas estão sendo impressas por planilha.</span><span class="sxs-lookup"><span data-stu-id="84e6e-150">The default direction to lay out pages when multiple pages are being printed per sheet.</span></span> <span data-ttu-id="84e6e-151">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="84e6e-151">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="84e6e-152">colorMode</span><span class="sxs-lookup"><span data-stu-id="84e6e-152">colorMode</span></span>|[<span data-ttu-id="84e6e-153">printColorMode</span><span class="sxs-lookup"><span data-stu-id="84e6e-153">printColorMode</span></span>](enums.md#printcolormode-values)|<span data-ttu-id="84e6e-154">O modo de cor padrão a ser usado ao imprimir o documento.</span><span class="sxs-lookup"><span data-stu-id="84e6e-154">The default color mode to use when printing the document.</span></span> <span data-ttu-id="84e6e-155">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="84e6e-155">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="84e6e-156">quality</span><span class="sxs-lookup"><span data-stu-id="84e6e-156">quality</span></span>|[<span data-ttu-id="84e6e-157">printQuality</span><span class="sxs-lookup"><span data-stu-id="84e6e-157">printQuality</span></span>](enums.md#printquality-values)|<span data-ttu-id="84e6e-158">A qualidade padrão a ser usada ao imprimir o documento.</span><span class="sxs-lookup"><span data-stu-id="84e6e-158">The default quality to use when printing the document.</span></span> <span data-ttu-id="84e6e-159">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="84e6e-159">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="84e6e-160">duplexMode</span><span class="sxs-lookup"><span data-stu-id="84e6e-160">duplexMode</span></span>|[<span data-ttu-id="84e6e-161">printDuplexMode</span><span class="sxs-lookup"><span data-stu-id="84e6e-161">printDuplexMode</span></span>](enums.md#printduplexmode-values)|<span data-ttu-id="84e6e-162">A configuração duplex padrão (com duas laterais) a ser usada ao imprimir um documento.</span><span class="sxs-lookup"><span data-stu-id="84e6e-162">The default duplex (double-sided) configuration to use when printing a document.</span></span> <span data-ttu-id="84e6e-163">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="84e6e-163">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="84e6e-164">dpi</span><span class="sxs-lookup"><span data-stu-id="84e6e-164">dpi</span></span>|<span data-ttu-id="84e6e-165">Int32</span><span class="sxs-lookup"><span data-stu-id="84e6e-165">Int32</span></span>|<span data-ttu-id="84e6e-166">A resolução padrão no DPI a ser usada ao imprimir o trabalho.</span><span class="sxs-lookup"><span data-stu-id="84e6e-166">The default resolution in DPI to use when printing the job.</span></span>|
|<span data-ttu-id="84e6e-167">scaling</span><span class="sxs-lookup"><span data-stu-id="84e6e-167">scaling</span></span>|[<span data-ttu-id="84e6e-168">printScaling</span><span class="sxs-lookup"><span data-stu-id="84e6e-168">printScaling</span></span>](enums.md#printscaling-values)|<span data-ttu-id="84e6e-169">Especifica como a impressora dimensiona os dados do documento para se ajustar à mídia solicitada.</span><span class="sxs-lookup"><span data-stu-id="84e6e-169">Specifies how the printer scales the document data to fit the requested media.</span></span> <span data-ttu-id="84e6e-170">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="84e6e-170">Valid values are described in the following table.</span></span>|

## <a name="relationships"></a><span data-ttu-id="84e6e-171">Relações</span><span class="sxs-lookup"><span data-stu-id="84e6e-171">Relationships</span></span>
<span data-ttu-id="84e6e-172">Nenhum</span><span class="sxs-lookup"><span data-stu-id="84e6e-172">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="84e6e-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="84e6e-173">JSON representation</span></span>
<span data-ttu-id="84e6e-174">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="84e6e-174">The following is a JSON representation of the resource.</span></span>
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

