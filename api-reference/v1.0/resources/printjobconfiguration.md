---
title: Tipo de recurso printJobConfiguration
description: Um grupo de configurações que uma impressora deve usar para imprimir um trabalho.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: f848b9274172113404a39f13e42c003643dfdf74
ms.sourcegitcommit: 6e7d9987a255f1bee04f196a4a7e37f56621bfb8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2021
ms.locfileid: "51944237"
---
# <a name="printjobconfiguration-resource-type"></a><span data-ttu-id="d27a6-103">Tipo de recurso printJobConfiguration</span><span class="sxs-lookup"><span data-stu-id="d27a6-103">printJobConfiguration resource type</span></span>

<span data-ttu-id="d27a6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d27a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="d27a6-105">Um grupo de configurações que uma impressora deve usar para imprimir um trabalho.</span><span class="sxs-lookup"><span data-stu-id="d27a6-105">A group of settings that a printer should use to print a job.</span></span>

## <a name="properties"></a><span data-ttu-id="d27a6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d27a6-106">Properties</span></span>
|<span data-ttu-id="d27a6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d27a6-107">Property</span></span>|<span data-ttu-id="d27a6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d27a6-108">Type</span></span>|<span data-ttu-id="d27a6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d27a6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d27a6-110">pageRanges</span><span class="sxs-lookup"><span data-stu-id="d27a6-110">pageRanges</span></span>|<span data-ttu-id="d27a6-111">[Coleção integerRange](integerrange.md)</span><span class="sxs-lookup"><span data-stu-id="d27a6-111">[integerRange](integerrange.md) collection</span></span>|<span data-ttu-id="d27a6-112">A página varia para imprimir.</span><span class="sxs-lookup"><span data-stu-id="d27a6-112">The page ranges to print.</span></span> <span data-ttu-id="d27a6-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d27a6-113">Read-only.</span></span>|
|<span data-ttu-id="d27a6-114">quality</span><span class="sxs-lookup"><span data-stu-id="d27a6-114">quality</span></span>|[<span data-ttu-id="d27a6-115">printQuality</span><span class="sxs-lookup"><span data-stu-id="d27a6-115">printQuality</span></span>](enums.md#printquality-values)|<span data-ttu-id="d27a6-116">A qualidade de impressão a ser usada ao imprimir o trabalho.</span><span class="sxs-lookup"><span data-stu-id="d27a6-116">The print quality to use when printing the job.</span></span> <span data-ttu-id="d27a6-117">Os valores válidos são descritos na tabela abaixo.</span><span class="sxs-lookup"><span data-stu-id="d27a6-117">Valid values are described in the table below.</span></span> <span data-ttu-id="d27a6-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d27a6-118">Read-only.</span></span>|
|<span data-ttu-id="d27a6-119">dpi</span><span class="sxs-lookup"><span data-stu-id="d27a6-119">dpi</span></span>|<span data-ttu-id="d27a6-120">Int32</span><span class="sxs-lookup"><span data-stu-id="d27a6-120">Int32</span></span>|<span data-ttu-id="d27a6-121">A resolução a ser usada ao imprimir o trabalho, expressa em pontos por polegada (DPI).</span><span class="sxs-lookup"><span data-stu-id="d27a6-121">The resolution to use when printing the job, expressed in dots per inch (DPI).</span></span> <span data-ttu-id="d27a6-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d27a6-122">Read-only.</span></span>|
|<span data-ttu-id="d27a6-123">feedOrientation</span><span class="sxs-lookup"><span data-stu-id="d27a6-123">feedOrientation</span></span>|<span data-ttu-id="d27a6-124">printerFeedOrientation</span><span class="sxs-lookup"><span data-stu-id="d27a6-124">printerFeedOrientation</span></span>|<span data-ttu-id="d27a6-125">A orientação a ser usada ao alimentar mídia na impressora.</span><span class="sxs-lookup"><span data-stu-id="d27a6-125">The orientation to use when feeding media into the printer.</span></span> <span data-ttu-id="d27a6-126">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="d27a6-126">Valid values are described in the following table.</span></span> <span data-ttu-id="d27a6-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d27a6-127">Read-only.</span></span>|
|<span data-ttu-id="d27a6-128">orientation</span><span class="sxs-lookup"><span data-stu-id="d27a6-128">orientation</span></span>|[<span data-ttu-id="d27a6-129">printOrientation</span><span class="sxs-lookup"><span data-stu-id="d27a6-129">printOrientation</span></span>](enums.md#printorientation-values)|<span data-ttu-id="d27a6-130">A configuração de orientação que a impressora deve usar ao imprimir o trabalho.</span><span class="sxs-lookup"><span data-stu-id="d27a6-130">The orientation setting the printer should use when printing the job.</span></span> <span data-ttu-id="d27a6-131">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="d27a6-131">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="d27a6-132">duplexMode</span><span class="sxs-lookup"><span data-stu-id="d27a6-132">duplexMode</span></span>|[<span data-ttu-id="d27a6-133">printDuplexMode</span><span class="sxs-lookup"><span data-stu-id="d27a6-133">printDuplexMode</span></span>](enums.md#printduplexmode-values)|<span data-ttu-id="d27a6-134">O modo duplex que a impressora deve usar ao imprimir o trabalho.</span><span class="sxs-lookup"><span data-stu-id="d27a6-134">The duplex mode the printer should use when printing the job.</span></span> <span data-ttu-id="d27a6-135">Os valores válidos são descritos na tabela abaixo.</span><span class="sxs-lookup"><span data-stu-id="d27a6-135">Valid values are described in the table below.</span></span> <span data-ttu-id="d27a6-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d27a6-136">Read-only.</span></span>|
|<span data-ttu-id="d27a6-137">copies</span><span class="sxs-lookup"><span data-stu-id="d27a6-137">copies</span></span>|<span data-ttu-id="d27a6-138">Int32</span><span class="sxs-lookup"><span data-stu-id="d27a6-138">Int32</span></span>|<span data-ttu-id="d27a6-139">O número de cópias que devem ser impressas.</span><span class="sxs-lookup"><span data-stu-id="d27a6-139">The number of copies that should be printed.</span></span> <span data-ttu-id="d27a6-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d27a6-140">Read-only.</span></span>|
|<span data-ttu-id="d27a6-141">colorMode</span><span class="sxs-lookup"><span data-stu-id="d27a6-141">colorMode</span></span>|[<span data-ttu-id="d27a6-142">printColorMode</span><span class="sxs-lookup"><span data-stu-id="d27a6-142">printColorMode</span></span>](enums.md#printcolormode-values)|<span data-ttu-id="d27a6-143">O modo de cor que a impressora deve usar para imprimir o trabalho.</span><span class="sxs-lookup"><span data-stu-id="d27a6-143">The color mode the printer should use to print the job.</span></span> <span data-ttu-id="d27a6-144">Os valores válidos são descritos na tabela abaixo.</span><span class="sxs-lookup"><span data-stu-id="d27a6-144">Valid values are described in the table below.</span></span> <span data-ttu-id="d27a6-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d27a6-145">Read-only.</span></span>|
|<span data-ttu-id="d27a6-146">inputBin</span><span class="sxs-lookup"><span data-stu-id="d27a6-146">inputBin</span></span>|<span data-ttu-id="d27a6-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d27a6-147">String</span></span>|<span data-ttu-id="d27a6-148">A bandeja de entrada (bandeja) a ser usada durante a impressão.</span><span class="sxs-lookup"><span data-stu-id="d27a6-148">The input bin (tray) to use when printing.</span></span> <span data-ttu-id="d27a6-149">Consulte os recursos da [impressora para](printercapabilities.md) uma lista de caixas de entrada com suporte.</span><span class="sxs-lookup"><span data-stu-id="d27a6-149">See the printer's [capabilities](printercapabilities.md) for a list of supported input bins.</span></span>|
|<span data-ttu-id="d27a6-150">outputBin</span><span class="sxs-lookup"><span data-stu-id="d27a6-150">outputBin</span></span>|<span data-ttu-id="d27a6-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d27a6-151">String</span></span>|<span data-ttu-id="d27a6-152">A lixeira de saída para colocar as impressões concluídas.</span><span class="sxs-lookup"><span data-stu-id="d27a6-152">The output bin to place completed prints into.</span></span> <span data-ttu-id="d27a6-153">Consulte os recursos da [impressora para](printercapabilities.md) uma lista de caixas de saída com suporte.</span><span class="sxs-lookup"><span data-stu-id="d27a6-153">See the printer's [capabilities](printercapabilities.md) for a list of supported output bins.</span></span>|
|<span data-ttu-id="d27a6-154">mediaSize</span><span class="sxs-lookup"><span data-stu-id="d27a6-154">mediaSize</span></span>|<span data-ttu-id="d27a6-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d27a6-155">String</span></span>|<span data-ttu-id="d27a6-156">O tamanho da mídia a ser usado ao imprimir.</span><span class="sxs-lookup"><span data-stu-id="d27a6-156">The media size to use when printing.</span></span> <span data-ttu-id="d27a6-157">Oferece suporte a nomes de tamanho padrão para tamanhos de mídia ISO e ANSI.</span><span class="sxs-lookup"><span data-stu-id="d27a6-157">Supports standard size names for ISO and ANSI media sizes.</span></span> <span data-ttu-id="d27a6-158">Valores válidos listados no tópico [printerCapabilities.](printercapabilities.md#mediasizes-values)</span><span class="sxs-lookup"><span data-stu-id="d27a6-158">Valid values listed in the [printerCapabilities](printercapabilities.md#mediasizes-values) topic.</span></span>|
|<span data-ttu-id="d27a6-159">margin</span><span class="sxs-lookup"><span data-stu-id="d27a6-159">margin</span></span>|[<span data-ttu-id="d27a6-160">printMargin</span><span class="sxs-lookup"><span data-stu-id="d27a6-160">printMargin</span></span>](printmargin.md)|<span data-ttu-id="d27a6-161">As configurações de margem a ser usadas ao imprimir.</span><span class="sxs-lookup"><span data-stu-id="d27a6-161">The margin settings to use when printing.</span></span>|
|<span data-ttu-id="d27a6-162">mediaType</span><span class="sxs-lookup"><span data-stu-id="d27a6-162">mediaType</span></span>|<span data-ttu-id="d27a6-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d27a6-163">String</span></span>|<span data-ttu-id="d27a6-164">O tipo de mídia padrão (como papel) para imprimir o documento.</span><span class="sxs-lookup"><span data-stu-id="d27a6-164">The default media (such as paper) type to print the document on.</span></span>|
|<span data-ttu-id="d27a6-165">finishings</span><span class="sxs-lookup"><span data-stu-id="d27a6-165">finishings</span></span>|<span data-ttu-id="d27a6-166">[Coleção printFinishing](enums.md#printfinishing-values)</span><span class="sxs-lookup"><span data-stu-id="d27a6-166">[printFinishing](enums.md#printfinishing-values) collection</span></span>|<span data-ttu-id="d27a6-167">Processos de término a ser usado ao imprimir.</span><span class="sxs-lookup"><span data-stu-id="d27a6-167">Finishing processes to use when printing.</span></span>|
|<span data-ttu-id="d27a6-168">pagesPerSheet</span><span class="sxs-lookup"><span data-stu-id="d27a6-168">pagesPerSheet</span></span>|<span data-ttu-id="d27a6-169">Int32</span><span class="sxs-lookup"><span data-stu-id="d27a6-169">Int32</span></span>|<span data-ttu-id="d27a6-170">O número de páginas de documento a ser impressa em cada planilha.</span><span class="sxs-lookup"><span data-stu-id="d27a6-170">The number of document pages to print on each sheet.</span></span>
|<span data-ttu-id="d27a6-171">multipageLayout</span><span class="sxs-lookup"><span data-stu-id="d27a6-171">multipageLayout</span></span>|[<span data-ttu-id="d27a6-172">printMultipageLayout</span><span class="sxs-lookup"><span data-stu-id="d27a6-172">printMultipageLayout</span></span>](enums.md#printmultipagelayout-values)|<span data-ttu-id="d27a6-173">A direção para colocar as páginas quando várias páginas estão sendo impressas por planilha.</span><span class="sxs-lookup"><span data-stu-id="d27a6-173">The direction to lay out pages when multiple pages are being printed per sheet.</span></span> <span data-ttu-id="d27a6-174">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="d27a6-174">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="d27a6-175">collate</span><span class="sxs-lookup"><span data-stu-id="d27a6-175">collate</span></span>|<span data-ttu-id="d27a6-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="d27a6-176">Boolean</span></span>|<span data-ttu-id="d27a6-177">Se a impressora deve colá-los para imprimir várias cópias de um documento de várias páginas.</span><span class="sxs-lookup"><span data-stu-id="d27a6-177">Whether the printer should collate pages wehen printing multiple copies of a multi-page document.</span></span>|
|<span data-ttu-id="d27a6-178">scaling</span><span class="sxs-lookup"><span data-stu-id="d27a6-178">scaling</span></span>|[<span data-ttu-id="d27a6-179">printScaling</span><span class="sxs-lookup"><span data-stu-id="d27a6-179">printScaling</span></span>](enums.md#printscaling-values)|<span data-ttu-id="d27a6-180">Especifica como a impressora deve dimensionar os dados do documento para se ajustar à mídia solicitada.</span><span class="sxs-lookup"><span data-stu-id="d27a6-180">Specifies how the printer should scale the document data to fit the requested media.</span></span> <span data-ttu-id="d27a6-181">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="d27a6-181">Valid values are described in the following table.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d27a6-182">Relações</span><span class="sxs-lookup"><span data-stu-id="d27a6-182">Relationships</span></span>
<span data-ttu-id="d27a6-183">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d27a6-183">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d27a6-184">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d27a6-184">JSON representation</span></span>
<span data-ttu-id="d27a6-185">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d27a6-185">The following is a JSON representation of the resource.</span></span>
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

