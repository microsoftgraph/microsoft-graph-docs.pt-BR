---
title: tipo de recurso printerDocumentConfiguration
description: Um grupo de configurações que uma impressora deve usar para imprimir um documento.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: ff1da92894f8854bcdee2ce24d7a9d5cef6288e7
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895484"
---
# <a name="printerdocumentconfiguration-resource-type"></a><span data-ttu-id="7a17a-103">tipo de recurso printerDocumentConfiguration</span><span class="sxs-lookup"><span data-stu-id="7a17a-103">printerDocumentConfiguration resource type</span></span>

<span data-ttu-id="7a17a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a17a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a17a-105">Um grupo de configurações que uma impressora deve usar para imprimir um documento.</span><span class="sxs-lookup"><span data-stu-id="7a17a-105">A group of settings that a printer should use to print a document.</span></span>

## <a name="properties"></a><span data-ttu-id="7a17a-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7a17a-106">Properties</span></span>
| <span data-ttu-id="7a17a-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a17a-107">Property</span></span>     | <span data-ttu-id="7a17a-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a17a-108">Type</span></span>        | <span data-ttu-id="7a17a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a17a-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7a17a-110">pageRanges</span><span class="sxs-lookup"><span data-stu-id="7a17a-110">pageRanges</span></span>|<span data-ttu-id="7a17a-111">coleção [printPageRange](printpagerange.md)</span><span class="sxs-lookup"><span data-stu-id="7a17a-111">[printPageRange](printpagerange.md) collection</span></span>|<span data-ttu-id="7a17a-112">Os intervalos de páginas a serem impressos.</span><span class="sxs-lookup"><span data-stu-id="7a17a-112">The page ranges to print.</span></span> <span data-ttu-id="7a17a-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7a17a-113">Read-only.</span></span>|
|<span data-ttu-id="7a17a-114">printQuality</span><span class="sxs-lookup"><span data-stu-id="7a17a-114">printQuality</span></span>|<span data-ttu-id="7a17a-115">printQuality</span><span class="sxs-lookup"><span data-stu-id="7a17a-115">printQuality</span></span>|<span data-ttu-id="7a17a-116">A qualidade de impressão a ser usada ao imprimir o trabalho.</span><span class="sxs-lookup"><span data-stu-id="7a17a-116">The print quality to use when printing the job.</span></span> <span data-ttu-id="7a17a-117">Os valores válidos são descritos na tabela abaixo.</span><span class="sxs-lookup"><span data-stu-id="7a17a-117">Valid values are described in the table below.</span></span> <span data-ttu-id="7a17a-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7a17a-118">Read-only.</span></span>|
|<span data-ttu-id="7a17a-119">printResolutionInDpi</span><span class="sxs-lookup"><span data-stu-id="7a17a-119">printResolutionInDpi</span></span>|<span data-ttu-id="7a17a-120">Int32</span><span class="sxs-lookup"><span data-stu-id="7a17a-120">Int32</span></span>|<span data-ttu-id="7a17a-121">A resolução a ser usada ao imprimir o trabalho, expresso em pontos por polegada (DPI).</span><span class="sxs-lookup"><span data-stu-id="7a17a-121">The resolution to use when printing the job, expressed in dots per inch (DPI).</span></span> <span data-ttu-id="7a17a-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7a17a-122">Read-only.</span></span>|
|<span data-ttu-id="7a17a-123">feedDirection</span><span class="sxs-lookup"><span data-stu-id="7a17a-123">feedDirection</span></span>|<span data-ttu-id="7a17a-124">printerFeedDirection</span><span class="sxs-lookup"><span data-stu-id="7a17a-124">printerFeedDirection</span></span>|<span data-ttu-id="7a17a-125">A direção a ser usada ao alimentar mídia na impressora.</span><span class="sxs-lookup"><span data-stu-id="7a17a-125">The direction to use when feeding media into the printer.</span></span> <span data-ttu-id="7a17a-126">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="7a17a-126">Valid values are described in the following table.</span></span> <span data-ttu-id="7a17a-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7a17a-127">Read-only.</span></span>|
|<span data-ttu-id="7a17a-128">orientation</span><span class="sxs-lookup"><span data-stu-id="7a17a-128">orientation</span></span>|<span data-ttu-id="7a17a-129">a reorientação</span><span class="sxs-lookup"><span data-stu-id="7a17a-129">printOrientation</span></span>|<span data-ttu-id="7a17a-130">A configuração de orientação que a impressora deve usar ao imprimir o trabalho.</span><span class="sxs-lookup"><span data-stu-id="7a17a-130">The orientation setting the printer should use when printing the job.</span></span> <span data-ttu-id="7a17a-131">Os valores válidos são descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="7a17a-131">Valid values are described in the following table.</span></span>|
|<span data-ttu-id="7a17a-132">duplexConfiguration</span><span class="sxs-lookup"><span data-stu-id="7a17a-132">duplexConfiguration</span></span>|<span data-ttu-id="7a17a-133">printDuplexConfiguration</span><span class="sxs-lookup"><span data-stu-id="7a17a-133">printDuplexConfiguration</span></span>|<span data-ttu-id="7a17a-134">A configuração duplex que a impressora deve usar ao imprimir o trabalho.</span><span class="sxs-lookup"><span data-stu-id="7a17a-134">The duplex configuration the printer should use when printing the job.</span></span> <span data-ttu-id="7a17a-135">Os valores válidos são descritos na tabela abaixo.</span><span class="sxs-lookup"><span data-stu-id="7a17a-135">Valid values are described in the table below.</span></span> <span data-ttu-id="7a17a-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7a17a-136">Read-only.</span></span>|
|<span data-ttu-id="7a17a-137">Copia</span><span class="sxs-lookup"><span data-stu-id="7a17a-137">copies</span></span>|<span data-ttu-id="7a17a-138">Int32</span><span class="sxs-lookup"><span data-stu-id="7a17a-138">Int32</span></span>|<span data-ttu-id="7a17a-139">O número de cópias que devem ser impressas.</span><span class="sxs-lookup"><span data-stu-id="7a17a-139">The number of copies that should be printed.</span></span> <span data-ttu-id="7a17a-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7a17a-140">Read-only.</span></span>|
|<span data-ttu-id="7a17a-141">colorConfiguration</span><span class="sxs-lookup"><span data-stu-id="7a17a-141">colorConfiguration</span></span>|<span data-ttu-id="7a17a-142">printColorConfiguration</span><span class="sxs-lookup"><span data-stu-id="7a17a-142">printColorConfiguration</span></span>|<span data-ttu-id="7a17a-143">A configuração de cor que a impressora deve usar para imprimir o trabalho.</span><span class="sxs-lookup"><span data-stu-id="7a17a-143">The color configuration the printer should use to print the job.</span></span> <span data-ttu-id="7a17a-144">Os valores válidos são descritos na tabela abaixo.</span><span class="sxs-lookup"><span data-stu-id="7a17a-144">Valid values are described in the table below.</span></span> <span data-ttu-id="7a17a-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7a17a-145">Read-only.</span></span>|

### <a name="printduplexconfiguration-values"></a><span data-ttu-id="7a17a-146">valores de printDuplexConfiguration</span><span class="sxs-lookup"><span data-stu-id="7a17a-146">printDuplexConfiguration values</span></span>

|<span data-ttu-id="7a17a-147">Membro</span><span class="sxs-lookup"><span data-stu-id="7a17a-147">Member</span></span>|<span data-ttu-id="7a17a-148">Valor</span><span class="sxs-lookup"><span data-stu-id="7a17a-148">Value</span></span>|<span data-ttu-id="7a17a-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a17a-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a17a-150">twoSidedLongEdge</span><span class="sxs-lookup"><span data-stu-id="7a17a-150">twoSidedLongEdge</span></span>|<span data-ttu-id="7a17a-151">,0</span><span class="sxs-lookup"><span data-stu-id="7a17a-151">0</span></span>|<span data-ttu-id="7a17a-152">A impressora imprimirá em frente e voltará os documentos ao longo da borda longa.</span><span class="sxs-lookup"><span data-stu-id="7a17a-152">The printer will print double-sided, and will flip documents along the long edge.</span></span>|
|<span data-ttu-id="7a17a-153">twoSidedShortEdge</span><span class="sxs-lookup"><span data-stu-id="7a17a-153">twoSidedShortEdge</span></span>|<span data-ttu-id="7a17a-154">1</span><span class="sxs-lookup"><span data-stu-id="7a17a-154">1</span></span>|<span data-ttu-id="7a17a-155">A impressora imprimirá em frente e voltará os documentos ao longo da borda curta.</span><span class="sxs-lookup"><span data-stu-id="7a17a-155">The printer will print double-sided, and will flip documents along the short edge.</span></span>|
|<span data-ttu-id="7a17a-156">oneSided</span><span class="sxs-lookup"><span data-stu-id="7a17a-156">oneSided</span></span>|<span data-ttu-id="7a17a-157">duas</span><span class="sxs-lookup"><span data-stu-id="7a17a-157">2</span></span>|<span data-ttu-id="7a17a-158">A impressora imprimirá um lado.</span><span class="sxs-lookup"><span data-stu-id="7a17a-158">The printer will print single-sided.</span></span>|

### <a name="printquality-values"></a><span data-ttu-id="7a17a-159">valores de PrintQuality</span><span class="sxs-lookup"><span data-stu-id="7a17a-159">printQuality values</span></span>

|<span data-ttu-id="7a17a-160">Member</span><span class="sxs-lookup"><span data-stu-id="7a17a-160">Member</span></span>|<span data-ttu-id="7a17a-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a17a-161">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7a17a-162">low</span><span class="sxs-lookup"><span data-stu-id="7a17a-162">low</span></span>|<span data-ttu-id="7a17a-163">A impressora imprimirá o trabalho usando a qualidade baixa (normalmente conhecida como "rascunho").</span><span class="sxs-lookup"><span data-stu-id="7a17a-163">The printer will print the job using low (commonly known as "draft") quality.</span></span>|
|<span data-ttu-id="7a17a-164">medium</span><span class="sxs-lookup"><span data-stu-id="7a17a-164">medium</span></span>|<span data-ttu-id="7a17a-165">A impressora imprimirá o trabalho usando o medim (comumente conhecido como qualidade "normal").</span><span class="sxs-lookup"><span data-stu-id="7a17a-165">The printer will print the job using medim (commonly known as "normal") quality.</span></span>|
|<span data-ttu-id="7a17a-166">high</span><span class="sxs-lookup"><span data-stu-id="7a17a-166">high</span></span>|<span data-ttu-id="7a17a-167">A impressora imprimirá o trabalho usando a qualidade alta (normalmente conhecida como "melhor" ou "boa").</span><span class="sxs-lookup"><span data-stu-id="7a17a-167">The printer will print the job using high (commonly known as "best" or "fine") quality.</span></span>|

## <a name="printerfeeddirection-values"></a><span data-ttu-id="7a17a-168">valores de printerFeedDirection</span><span class="sxs-lookup"><span data-stu-id="7a17a-168">printerFeedDirection values</span></span>

|<span data-ttu-id="7a17a-169">Member</span><span class="sxs-lookup"><span data-stu-id="7a17a-169">Member</span></span>|<span data-ttu-id="7a17a-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a17a-170">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7a17a-171">longEdgeFirst</span><span class="sxs-lookup"><span data-stu-id="7a17a-171">longEdgeFirst</span></span>|<span data-ttu-id="7a17a-172">A impressora consumirá planilhas da bandeja ativa na orientação "paisagem", com a borda longa da planilha primeiro.</span><span class="sxs-lookup"><span data-stu-id="7a17a-172">The printer will consume sheets from the active tray in "landscape" orientation, with the long edge of the sheet first.</span></span>|
|<span data-ttu-id="7a17a-173">shortEdgeFirst</span><span class="sxs-lookup"><span data-stu-id="7a17a-173">shortEdgeFirst</span></span>|<span data-ttu-id="7a17a-174">A impressora consumirá planilhas da bandeja ativa na orientação "retrato", com a borda curta da planilha primeiro.</span><span class="sxs-lookup"><span data-stu-id="7a17a-174">The printer will consume sheets from the active tray in "portrait" orientation, with the short edge of the sheet first.</span></span>|

## <a name="printorientation-values"></a><span data-ttu-id="7a17a-175">valores de reorientação</span><span class="sxs-lookup"><span data-stu-id="7a17a-175">printOrientation values</span></span>

|<span data-ttu-id="7a17a-176">Membro</span><span class="sxs-lookup"><span data-stu-id="7a17a-176">Member</span></span>|<span data-ttu-id="7a17a-177">Valor</span><span class="sxs-lookup"><span data-stu-id="7a17a-177">Value</span></span>|<span data-ttu-id="7a17a-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a17a-178">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a17a-179">modos</span><span class="sxs-lookup"><span data-stu-id="7a17a-179">portrait</span></span>|<span data-ttu-id="7a17a-180">3D</span><span class="sxs-lookup"><span data-stu-id="7a17a-180">3</span></span>|<span data-ttu-id="7a17a-181">A impressora imprimirá impressões na orientação "retrato".</span><span class="sxs-lookup"><span data-stu-id="7a17a-181">The printer will print impressions in the "portrait" orientation.</span></span>|
|<span data-ttu-id="7a17a-182">paisagens</span><span class="sxs-lookup"><span data-stu-id="7a17a-182">landscape</span></span>|<span data-ttu-id="7a17a-183">4 </span><span class="sxs-lookup"><span data-stu-id="7a17a-183">4</span></span>|<span data-ttu-id="7a17a-184">A impressora imprimirá impressões na orientação "paisagem".</span><span class="sxs-lookup"><span data-stu-id="7a17a-184">The printer will print impressions in the "landscape" orientation.</span></span>|
|<span data-ttu-id="7a17a-185">reverseLandscape</span><span class="sxs-lookup"><span data-stu-id="7a17a-185">reverseLandscape</span></span>|<span data-ttu-id="7a17a-186">5 </span><span class="sxs-lookup"><span data-stu-id="7a17a-186">5</span></span>|<span data-ttu-id="7a17a-187">A impressora imprimirá impressões na orientação "paisagem reversa".</span><span class="sxs-lookup"><span data-stu-id="7a17a-187">The printer will print impressions in the "reverse landscape" orientation.</span></span>|
|<span data-ttu-id="7a17a-188">reversePortrait</span><span class="sxs-lookup"><span data-stu-id="7a17a-188">reversePortrait</span></span>|<span data-ttu-id="7a17a-189">6 </span><span class="sxs-lookup"><span data-stu-id="7a17a-189">6</span></span>|<span data-ttu-id="7a17a-190">A impressora imprimirá impressões na orientação "retrato reverso".</span><span class="sxs-lookup"><span data-stu-id="7a17a-190">The printer will print impressions in the "reverse portrait" orientation.</span></span>|

### <a name="printcolorconfiguration-values"></a><span data-ttu-id="7a17a-191">valores de printColorConfiguration</span><span class="sxs-lookup"><span data-stu-id="7a17a-191">printColorConfiguration values</span></span>

|<span data-ttu-id="7a17a-192">Membro</span><span class="sxs-lookup"><span data-stu-id="7a17a-192">Member</span></span>|<span data-ttu-id="7a17a-193">Valor</span><span class="sxs-lookup"><span data-stu-id="7a17a-193">Value</span></span>|<span data-ttu-id="7a17a-194">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a17a-194">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a17a-195">blackAndWhite</span><span class="sxs-lookup"><span data-stu-id="7a17a-195">blackAndWhite</span></span>|<span data-ttu-id="7a17a-196">,0</span><span class="sxs-lookup"><span data-stu-id="7a17a-196">0</span></span>|<span data-ttu-id="7a17a-197">Preto e branco (Use apenas o material de marcador preto).</span><span class="sxs-lookup"><span data-stu-id="7a17a-197">Black and white (use black marker material only.)</span></span>|
|<span data-ttu-id="7a17a-198">escala</span><span class="sxs-lookup"><span data-stu-id="7a17a-198">grayscale</span></span>|<span data-ttu-id="7a17a-199">1</span><span class="sxs-lookup"><span data-stu-id="7a17a-199">1</span></span>|<span data-ttu-id="7a17a-200">Escala de cinza (pode usar algum material de marcador de cor.)</span><span class="sxs-lookup"><span data-stu-id="7a17a-200">Grayscale (may use some color marker material.)</span></span>|
|<span data-ttu-id="7a17a-201">color</span><span class="sxs-lookup"><span data-stu-id="7a17a-201">color</span></span>|<span data-ttu-id="7a17a-202">duas</span><span class="sxs-lookup"><span data-stu-id="7a17a-202">2</span></span>|<span data-ttu-id="7a17a-203">Color (use qualquer combinação de materiais de marcador para criar uma impressão colorida).</span><span class="sxs-lookup"><span data-stu-id="7a17a-203">Color (use any combination of marker materials to create a color impression).</span></span>|
|<span data-ttu-id="7a17a-204">Automático</span><span class="sxs-lookup"><span data-stu-id="7a17a-204">auto</span></span>|<span data-ttu-id="7a17a-205">3D</span><span class="sxs-lookup"><span data-stu-id="7a17a-205">3</span></span>|<span data-ttu-id="7a17a-206">Permitir que a impressora decida qual modo de cor usar.</span><span class="sxs-lookup"><span data-stu-id="7a17a-206">Let the printer decide which color mode to use.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7a17a-207">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7a17a-207">JSON representation</span></span>

<span data-ttu-id="7a17a-208">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7a17a-208">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerDocumentConfiguration"
}-->

```json
{
  "pageRanges": [{"@odata.type": "microsoft.graph.printPageRange"}],
  "printQuality": "String",
  "printResolutionInDpi": 123456,
  "feedDirection": "String",
  "orientation": "String",
  "duplexConfiguration": "String",
  "copies": 123456,
  "colorConfiguration": "String",
}

```
