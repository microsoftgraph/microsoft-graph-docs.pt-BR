---
title: Tipo de recurso printJobConfiguration
description: Um grupo de configurações que uma impressora deve usar para imprimir um trabalho.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 1e12541bd4426dca1e0d7b48b0e3bcbd9e2bb7ea
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517038"
---
# <a name="printjobconfiguration-resource-type"></a><span data-ttu-id="27770-103">Tipo de recurso printJobConfiguration</span><span class="sxs-lookup"><span data-stu-id="27770-103">printJobConfiguration resource type</span></span>

<span data-ttu-id="27770-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27770-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="27770-105">Um grupo de configurações que uma impressora deve usar para imprimir um trabalho.</span><span class="sxs-lookup"><span data-stu-id="27770-105">A group of settings that a printer should use to print a job.</span></span>

## <a name="properties"></a><span data-ttu-id="27770-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="27770-106">Properties</span></span>
|<span data-ttu-id="27770-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27770-107">Property</span></span>|<span data-ttu-id="27770-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="27770-108">Type</span></span>|<span data-ttu-id="27770-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="27770-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27770-110">pageRanges</span><span class="sxs-lookup"><span data-stu-id="27770-110">pageRanges</span></span>|<span data-ttu-id="27770-111">[Coleção integerRange](integerrange.md)</span><span class="sxs-lookup"><span data-stu-id="27770-111">[integerRange](integerrange.md) collection</span></span>|<span data-ttu-id="27770-112">A página varia para imprimir.</span><span class="sxs-lookup"><span data-stu-id="27770-112">The page ranges to print.</span></span> <span data-ttu-id="27770-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="27770-113">Read-only.</span></span>|
|<span data-ttu-id="27770-114">quality</span><span class="sxs-lookup"><span data-stu-id="27770-114">quality</span></span>|[<span data-ttu-id="27770-115">printQuality</span><span class="sxs-lookup"><span data-stu-id="27770-115">printQuality</span></span>](enums.md#printquality-values)|<span data-ttu-id="27770-116">A qualidade de impressão a ser usada ao imprimir o trabalho.</span><span class="sxs-lookup"><span data-stu-id="27770-116">The print quality to use when printing the job.</span></span> <span data-ttu-id="27770-117">Os valores válidos são descritos na tabela abaixo.</span><span class="sxs-lookup"><span data-stu-id="27770-117">Valid values are described in the table below.</span></span> <span data-ttu-id="27770-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="27770-118">Read-only.</span></span>|
|<span data-ttu-id="27770-119">dpi</span><span class="sxs-lookup"><span data-stu-id="27770-119">dpi</span></span>|<span data-ttu-id="27770-120">Int32</span><span class="sxs-lookup"><span data-stu-id="27770-120">Int32</span></span>|<span data-ttu-id="27770-121">A resolução a ser usada ao imprimir o trabalho, expressa em pontos por polegada (DPI).</span><span class="sxs-lookup"><span data-stu-id="27770-121">The resolution to use when printing the job, expressed in dots per inch (DPI).</span></span> <span data-ttu-id="27770-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="27770-122">Read-only.</span></span>|
|<span data-ttu-id="27770-123">feedOrientation</span><span class="sxs-lookup"><span data-stu-id="27770-123">feedOrientation</span></span>|<span data-ttu-id="27770-124">printerFeedOrientation</span><span class="sxs-lookup"><span data-stu-id="27770-124">printerFeedOrientation</span></span>|<span data-ttu-id="27770-125">A orientação a ser usada ao alimentar mídia na impressora.</span><span class="sxs-lookup"><span data-stu-id="27770-125">The orientation to use when feeding media into the printer.</span></span> <span data-ttu-id="27770-126">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="27770-126">Valid values are described in the following table.</span></span> <span data-ttu-id="27770-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="27770-127">Read-only.</span></span>|
|<span data-ttu-id="27770-128">orientation</span><span class="sxs-lookup"><span data-stu-id="27770-128">orientation</span></span>|[<span data-ttu-id="27770-129">printOrientation</span><span class="sxs-lookup"><span data-stu-id="27770-129">printOrientation</span></span>](enums.md#printorientation-values)|<span data-ttu-id="27770-130">A configuração de orientação que a impressora deve usar ao imprimir o trabalho.</span><span class="sxs-lookup"><span data-stu-id="27770-130">The orientation setting the printer should use when printing the job.</span></span> <span data-ttu-id="27770-131">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="27770-131">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="27770-132">duplexMode</span><span class="sxs-lookup"><span data-stu-id="27770-132">duplexMode</span></span>|[<span data-ttu-id="27770-133">printDuplexMode</span><span class="sxs-lookup"><span data-stu-id="27770-133">printDuplexMode</span></span>](enums.md#printduplexmode-values)|<span data-ttu-id="27770-134">O modo duplex que a impressora deve usar ao imprimir o trabalho.</span><span class="sxs-lookup"><span data-stu-id="27770-134">The duplex mode the printer should use when printing the job.</span></span> <span data-ttu-id="27770-135">Os valores válidos são descritos na tabela abaixo.</span><span class="sxs-lookup"><span data-stu-id="27770-135">Valid values are described in the table below.</span></span> <span data-ttu-id="27770-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="27770-136">Read-only.</span></span>|
|<span data-ttu-id="27770-137">copies</span><span class="sxs-lookup"><span data-stu-id="27770-137">copies</span></span>|<span data-ttu-id="27770-138">Int32</span><span class="sxs-lookup"><span data-stu-id="27770-138">Int32</span></span>|<span data-ttu-id="27770-139">O número de cópias que devem ser impressas.</span><span class="sxs-lookup"><span data-stu-id="27770-139">The number of copies that should be printed.</span></span> <span data-ttu-id="27770-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="27770-140">Read-only.</span></span>|
|<span data-ttu-id="27770-141">colorMode</span><span class="sxs-lookup"><span data-stu-id="27770-141">colorMode</span></span>|[<span data-ttu-id="27770-142">printColorMode</span><span class="sxs-lookup"><span data-stu-id="27770-142">printColorMode</span></span>](enums.md#printcolormode-values)|<span data-ttu-id="27770-143">O modo de cor que a impressora deve usar para imprimir o trabalho.</span><span class="sxs-lookup"><span data-stu-id="27770-143">The color mode the printer should use to print the job.</span></span> <span data-ttu-id="27770-144">Os valores válidos são descritos na tabela abaixo.</span><span class="sxs-lookup"><span data-stu-id="27770-144">Valid values are described in the table below.</span></span> <span data-ttu-id="27770-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="27770-145">Read-only.</span></span>|
|<span data-ttu-id="27770-146">inputBin</span><span class="sxs-lookup"><span data-stu-id="27770-146">inputBin</span></span>|<span data-ttu-id="27770-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="27770-147">String</span></span>|<span data-ttu-id="27770-148">A bandeja de entrada (bandeja) a ser usada durante a impressão.</span><span class="sxs-lookup"><span data-stu-id="27770-148">The input bin (tray) to use when printing.</span></span> <span data-ttu-id="27770-149">Consulte os recursos da [impressora para](printercapabilities.md) uma lista de caixas de entrada com suporte.</span><span class="sxs-lookup"><span data-stu-id="27770-149">See the printer's [capabilities](printercapabilities.md) for a list of supported input bins.</span></span>|
|<span data-ttu-id="27770-150">outputBin</span><span class="sxs-lookup"><span data-stu-id="27770-150">outputBin</span></span>|<span data-ttu-id="27770-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="27770-151">String</span></span>|<span data-ttu-id="27770-152">A lixeira de saída para colocar as impressões concluídas.</span><span class="sxs-lookup"><span data-stu-id="27770-152">The output bin to place completed prints into.</span></span> <span data-ttu-id="27770-153">Consulte os recursos da [impressora para](printercapabilities.md) uma lista de caixas de saída com suporte.</span><span class="sxs-lookup"><span data-stu-id="27770-153">See the printer's [capabilities](printercapabilities.md) for a list of supported output bins.</span></span>|
|<span data-ttu-id="27770-154">mediaSize</span><span class="sxs-lookup"><span data-stu-id="27770-154">mediaSize</span></span>|<span data-ttu-id="27770-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="27770-155">String</span></span>|<span data-ttu-id="27770-156">O tamanho da mídia a ser usado ao imprimir.</span><span class="sxs-lookup"><span data-stu-id="27770-156">The media sizeto use when printing.</span></span> <span data-ttu-id="27770-157">Oferece suporte a nomes de tamanho padrão para tamanhos de mídia ISO e ANSI, juntamente com todos os tamanhos personalizados suportados pela impressora associada.</span><span class="sxs-lookup"><span data-stu-id="27770-157">Supports standard size names for ISO and ANSI media sizes, along with any custom sizes supported by the associated printer.</span></span>|
|<span data-ttu-id="27770-158">margin</span><span class="sxs-lookup"><span data-stu-id="27770-158">margin</span></span>|[<span data-ttu-id="27770-159">printMargin</span><span class="sxs-lookup"><span data-stu-id="27770-159">printMargin</span></span>](printmargin.md)|<span data-ttu-id="27770-160">As configurações de margem a ser usadas ao imprimir.</span><span class="sxs-lookup"><span data-stu-id="27770-160">The margin settings to use when printing.</span></span>|
|<span data-ttu-id="27770-161">mediaType</span><span class="sxs-lookup"><span data-stu-id="27770-161">mediaType</span></span>|<span data-ttu-id="27770-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="27770-162">String</span></span>|<span data-ttu-id="27770-163">O tipo de mídia padrão (como papel) para imprimir o documento.</span><span class="sxs-lookup"><span data-stu-id="27770-163">The default media (such as paper) type to print the document on.</span></span> <span data-ttu-id="27770-164">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="27770-164">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="27770-165">finishings</span><span class="sxs-lookup"><span data-stu-id="27770-165">finishings</span></span>|<span data-ttu-id="27770-166">[Coleção printFinishing](enums.md#printfinishing-values)</span><span class="sxs-lookup"><span data-stu-id="27770-166">[printFinishing](enums.md#printfinishing-values) collection</span></span>|<span data-ttu-id="27770-167">Processos de término a ser usado ao imprimir.</span><span class="sxs-lookup"><span data-stu-id="27770-167">Finishing processes to use when printing.</span></span>|
|<span data-ttu-id="27770-168">pagesPerSheet</span><span class="sxs-lookup"><span data-stu-id="27770-168">pagesPerSheet</span></span>|<span data-ttu-id="27770-169">Int32</span><span class="sxs-lookup"><span data-stu-id="27770-169">Int32</span></span>|<span data-ttu-id="27770-170">O número de páginas de documento a ser impressa em cada planilha.</span><span class="sxs-lookup"><span data-stu-id="27770-170">The number of document pages to print on each sheet.</span></span>
|<span data-ttu-id="27770-171">multipageLayout</span><span class="sxs-lookup"><span data-stu-id="27770-171">multipageLayout</span></span>|[<span data-ttu-id="27770-172">printMultipageLayout</span><span class="sxs-lookup"><span data-stu-id="27770-172">printMultipageLayout</span></span>](enums.md#printmultipagelayout-values)|<span data-ttu-id="27770-173">A direção para colocar as páginas quando várias páginas estão sendo impressas por planilha.</span><span class="sxs-lookup"><span data-stu-id="27770-173">The direction to lay out pages when multiple pages are being printed per sheet.</span></span> <span data-ttu-id="27770-174">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="27770-174">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="27770-175">collate</span><span class="sxs-lookup"><span data-stu-id="27770-175">collate</span></span>|<span data-ttu-id="27770-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="27770-176">Boolean</span></span>|<span data-ttu-id="27770-177">Se a impressora deve colá-los para imprimir várias cópias de um documento de várias páginas.</span><span class="sxs-lookup"><span data-stu-id="27770-177">Whether the printer should collate pages wehen printing multiple copies of a multi-page document.</span></span>|
|<span data-ttu-id="27770-178">scaling</span><span class="sxs-lookup"><span data-stu-id="27770-178">scaling</span></span>|[<span data-ttu-id="27770-179">printScaling</span><span class="sxs-lookup"><span data-stu-id="27770-179">printScaling</span></span>](enums.md#printscaling-values)|<span data-ttu-id="27770-180">Especifica como a impressora deve dimensionar os dados do documento para se ajustar à mídia solicitada.</span><span class="sxs-lookup"><span data-stu-id="27770-180">Specifies how the printer should scale the document data to fit the requested media.</span></span> <span data-ttu-id="27770-181">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="27770-181">Valid values are described in the following table.</span></span>|

## <a name="relationships"></a><span data-ttu-id="27770-182">Relações</span><span class="sxs-lookup"><span data-stu-id="27770-182">Relationships</span></span>
<span data-ttu-id="27770-183">Nenhum</span><span class="sxs-lookup"><span data-stu-id="27770-183">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="27770-184">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="27770-184">JSON representation</span></span>
<span data-ttu-id="27770-185">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="27770-185">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printJobConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printJobConfiguration",
  "pageRanges": [
    {
      "@odata.type": "microsoft.graph.integerRange"
    }
  ],
  "quality": "String",
  "dpi": "Integer",
  "feedOrientation": "String",
  "orientation": "String",
  "duplexMode": "String",
  "copies": "Integer",
  "colorMode": "String",
  "inputBin": "String",
  "outputBin": "String",
  "mediaSize": "String",
  "margin": {
    "@odata.type": "microsoft.graph.printMargin"
  },
  "mediaType": "String",
  "finishings": [
    "String"
  ],
  "pagesPerSheet": "Integer",
  "multipageLayout": "String",
  "collate": "Boolean",
  "scaling": "String",
  "fitPdfToPage": "Boolean"
}
```

