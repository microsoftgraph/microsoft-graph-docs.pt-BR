---
author: JeremyKelley
description: Aqui está uma representação JSON de um recurso columnDefinition.
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: aab34ebe8a0cb7539775ba3e7b07e8ad7b3c357b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444333"
---
# <a name="columndefinition-resource-type"></a><span data-ttu-id="8d328-103">Tipo de recurso columnDefinition</span><span class="sxs-lookup"><span data-stu-id="8d328-103">columnDefinition resource type</span></span>

<span data-ttu-id="8d328-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d328-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="8d328-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8d328-105">JSON representation</span></span>

<span data-ttu-id="8d328-106">Aqui está uma representação JSON de um recurso columnDefinition.</span><span class="sxs-lookup"><span data-stu-id="8d328-106">Here is a JSON representation of a columnDefinition resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.columnDefinition"
}-->

```json
{
  "columnGroup": "string",
  "description": "description",
  "displayName": "friendly name",
  "enforceUniqueValues": true,
  "hidden": false,
  "id": "string",
  "indexed": true,
  "name": "staticNameForApi",
  "readOnly": false,
  "required": false,
  "boolean": { "@odata.type": "microsoft.graph.booleanColumn" },
  "calculated": { "@odata.type": "microsoft.graph.calculatedColumn" },
  "choice": { "@odata.type": "microsoft.graph.choiceColumn" },
  "currency": { "@odata.type": "microsoft.graph.currencyColumn" },
  "dateTime": { "@odata.type": "microsoft.graph.dateTimeColumn" },
  "defaultValue": { "@odata.type": "microsoft.graph.defaultColumnValue" },
  "geolocation": { "@odata.type": "microsoft.graph.geolocationColumn" },
  "lookup": { "@odata.type": "microsoft.graph.lookupColumn" },
  "number": { "@odata.type": "microsoft.graph.numberColumn" },
  "personOrGroup": { "@odata.type": "microsoft.graph.personOrGroupColumn" },
  "text": { "@odata.type": "microsoft.graph.textColumn" },
  "isDeletable" : false,
  "propagateChanges": false,
  "isReorderable": false,
  "isSealed": false,
  "validation": { "@odata.type": "microsoft.graph.columnValidation" },
  "hyperlinkOrPicture": { "@odata.type": "microsoft.graph.hyperlinkOrPictureColumn" },
  "term": { "@odata.type": "microsoft.graph.termColumn" },
  "sourceContentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },
  "thumbnail": { "@odata.type": "microsoft.graph.thumbnailColumn" },
  "type": { "@odata.type": "microsoft.graph.columnTypes" },
  "contentApprovalStatus": { "@odata.type": "microsoft.graph.contentApprovalStatusColumn" }
}
```

## <a name="properties"></a><span data-ttu-id="8d328-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8d328-107">Properties</span></span>

<span data-ttu-id="8d328-108">As colunas podem conter dados de vários tipos.</span><span class="sxs-lookup"><span data-stu-id="8d328-108">Columns can hold data of various types.</span></span>
<span data-ttu-id="8d328-109">As propriedades a seguir indicam qual tipo de dados uma coluna armazena, bem como configurações adicionais para esses dados.</span><span class="sxs-lookup"><span data-stu-id="8d328-109">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="8d328-110">As propriedades relacionadas ao tipo (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) são mutuamente exclusivas. Uma coluna só pode ter uma delas especificada.</span><span class="sxs-lookup"><span data-stu-id="8d328-110">The type-related properties (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="8d328-111">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="8d328-111">Property name</span></span>           | <span data-ttu-id="8d328-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d328-112">Type</span></span>    | <span data-ttu-id="8d328-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d328-113">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="8d328-114">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="8d328-114">**columnGroup**</span></span>         | <span data-ttu-id="8d328-115">string</span><span class="sxs-lookup"><span data-stu-id="8d328-115">string</span></span>  | <span data-ttu-id="8d328-116">Para colunas de site, o nome do grupo ao qual esta coluna pertence.</span><span class="sxs-lookup"><span data-stu-id="8d328-116">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="8d328-117">Ajuda a organizar as colunas relacionadas.</span><span class="sxs-lookup"><span data-stu-id="8d328-117">Helps organize related columns.</span></span>
| <span data-ttu-id="8d328-118">**description**</span><span class="sxs-lookup"><span data-stu-id="8d328-118">**description**</span></span>         | <span data-ttu-id="8d328-119">string</span><span class="sxs-lookup"><span data-stu-id="8d328-119">string</span></span>  | <span data-ttu-id="8d328-120">A descrição voltado para o usuário da coluna.</span><span class="sxs-lookup"><span data-stu-id="8d328-120">The user-facing description of the column.</span></span>
| <span data-ttu-id="8d328-121">**displayName**</span><span class="sxs-lookup"><span data-stu-id="8d328-121">**displayName**</span></span>         | <span data-ttu-id="8d328-122">string</span><span class="sxs-lookup"><span data-stu-id="8d328-122">string</span></span>  | <span data-ttu-id="8d328-123">O nome voltado para o usuário da coluna.</span><span class="sxs-lookup"><span data-stu-id="8d328-123">The user-facing name of the column.</span></span>
| <span data-ttu-id="8d328-124">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="8d328-124">**enforceUniqueValues**</span></span> | <span data-ttu-id="8d328-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d328-125">Boolean</span></span> | <span data-ttu-id="8d328-126">Se for verdadeiro, esse mesmo valor não constará em dois itens de lista nessa coluna.</span><span class="sxs-lookup"><span data-stu-id="8d328-126">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="8d328-127">**hidden**</span><span class="sxs-lookup"><span data-stu-id="8d328-127">**hidden**</span></span>              | <span data-ttu-id="8d328-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d328-128">Boolean</span></span> | <span data-ttu-id="8d328-129">Especifica se a coluna é exibida na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="8d328-129">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="8d328-130">**id**</span><span class="sxs-lookup"><span data-stu-id="8d328-130">**id**</span></span>                  | <span data-ttu-id="8d328-131">string</span><span class="sxs-lookup"><span data-stu-id="8d328-131">string</span></span>  | <span data-ttu-id="8d328-132">O identificador exclusivo da coluna.</span><span class="sxs-lookup"><span data-stu-id="8d328-132">The unique identifier for the column.</span></span>
| <span data-ttu-id="8d328-133">**indexed**</span><span class="sxs-lookup"><span data-stu-id="8d328-133">**indexed**</span></span>             | <span data-ttu-id="8d328-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d328-134">Boolean</span></span> | <span data-ttu-id="8d328-135">Especifica se os valores da coluna podem ser usados para classificação e pesquisa.</span><span class="sxs-lookup"><span data-stu-id="8d328-135">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="8d328-136">**name**</span><span class="sxs-lookup"><span data-stu-id="8d328-136">**name**</span></span>                | <span data-ttu-id="8d328-137">string</span><span class="sxs-lookup"><span data-stu-id="8d328-137">string</span></span>  | <span data-ttu-id="8d328-138">O nome voltado para a API da coluna, conforme ele aparece nos [campos][] em uma [listItem][].</span><span class="sxs-lookup"><span data-stu-id="8d328-138">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="8d328-139">Para o nome voltado ao usuário, consulte **displayName**.</span><span class="sxs-lookup"><span data-stu-id="8d328-139">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="8d328-140">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="8d328-140">**readOnly**</span></span>            | <span data-ttu-id="8d328-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d328-141">Boolean</span></span>    | <span data-ttu-id="8d328-142">Especifica se os valores da coluna podem ser modificados.</span><span class="sxs-lookup"><span data-stu-id="8d328-142">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="8d328-143">**required**</span><span class="sxs-lookup"><span data-stu-id="8d328-143">**required**</span></span>            | <span data-ttu-id="8d328-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d328-144">Boolean</span></span> | <span data-ttu-id="8d328-145">Especifica se o valor da coluna não é opcional.</span><span class="sxs-lookup"><span data-stu-id="8d328-145">Specifies whether the column value is not optional.</span></span>
| <span data-ttu-id="8d328-146">**boolean**</span><span class="sxs-lookup"><span data-stu-id="8d328-146">**boolean**</span></span>       | <span data-ttu-id="8d328-147">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="8d328-147">[booleanColumn][]</span></span>       | <span data-ttu-id="8d328-148">Esta coluna armazena valores boolianos.</span><span class="sxs-lookup"><span data-stu-id="8d328-148">This column stores boolean values.</span></span>
| <span data-ttu-id="8d328-149">**calculated**</span><span class="sxs-lookup"><span data-stu-id="8d328-149">**calculated**</span></span>    | <span data-ttu-id="8d328-150">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="8d328-150">[calculatedColumn][]</span></span>    | <span data-ttu-id="8d328-151">Os dados dessa coluna são calculados com base em outras colunas.</span><span class="sxs-lookup"><span data-stu-id="8d328-151">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="8d328-152">**choice**</span><span class="sxs-lookup"><span data-stu-id="8d328-152">**choice**</span></span>        | <span data-ttu-id="8d328-153">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="8d328-153">[choiceColumn][]</span></span>        | <span data-ttu-id="8d328-154">Esta coluna armazena dados de uma lista de opções.</span><span class="sxs-lookup"><span data-stu-id="8d328-154">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="8d328-155">**currency**</span><span class="sxs-lookup"><span data-stu-id="8d328-155">**currency**</span></span>      | <span data-ttu-id="8d328-156">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="8d328-156">[currencyColumn][]</span></span>      | <span data-ttu-id="8d328-157">Esta coluna armazena valores monetários.</span><span class="sxs-lookup"><span data-stu-id="8d328-157">This column stores currency values.</span></span>
| <span data-ttu-id="8d328-158">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="8d328-158">**dateTime**</span></span>      | <span data-ttu-id="8d328-159">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="8d328-159">[dateTimeColumn][]</span></span>      | <span data-ttu-id="8d328-160">Esta coluna armazena valores de datetime.</span><span class="sxs-lookup"><span data-stu-id="8d328-160">This column stores DateTime values.</span></span>
| <span data-ttu-id="8d328-161">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="8d328-161">**defaultValue**</span></span>  | <span data-ttu-id="8d328-162">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="8d328-162">[defaultColumnValue][]</span></span>  | <span data-ttu-id="8d328-163">O valor padrão dessa coluna.</span><span class="sxs-lookup"><span data-stu-id="8d328-163">The default value for this column.</span></span>
| <span data-ttu-id="8d328-164">**geolocalização**</span><span class="sxs-lookup"><span data-stu-id="8d328-164">**geolocation**</span></span>   | <span data-ttu-id="8d328-165">[geolocationColumn][]</span><span class="sxs-lookup"><span data-stu-id="8d328-165">[geolocationColumn][]</span></span>   | <span data-ttu-id="8d328-166">Esta coluna armazena uma localização geográfica.</span><span class="sxs-lookup"><span data-stu-id="8d328-166">This column stores a geolocation.</span></span>
| <span data-ttu-id="8d328-167">**lookup**</span><span class="sxs-lookup"><span data-stu-id="8d328-167">**lookup**</span></span>        | <span data-ttu-id="8d328-168">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="8d328-168">[lookupColumn][]</span></span>        | <span data-ttu-id="8d328-169">Os dados dessa coluna são procurados por outra fonte no site.</span><span class="sxs-lookup"><span data-stu-id="8d328-169">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="8d328-170">**number**</span><span class="sxs-lookup"><span data-stu-id="8d328-170">**number**</span></span>        | <span data-ttu-id="8d328-171">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="8d328-171">[numberColumn][]</span></span>        | <span data-ttu-id="8d328-172">Esta coluna armazena valores numéricos.</span><span class="sxs-lookup"><span data-stu-id="8d328-172">This column stores number values.</span></span>
| <span data-ttu-id="8d328-173">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="8d328-173">**personOrGroup**</span></span> | <span data-ttu-id="8d328-174">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="8d328-174">[personOrGroupColumn][]</span></span> | <span data-ttu-id="8d328-175">Esta coluna armazena valores de Pessoa ou Grupo.</span><span class="sxs-lookup"><span data-stu-id="8d328-175">This column stores Person or Group values.</span></span>
| <span data-ttu-id="8d328-176">**text**</span><span class="sxs-lookup"><span data-stu-id="8d328-176">**text**</span></span>          | <span data-ttu-id="8d328-177">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="8d328-177">[textColumn][]</span></span>          | <span data-ttu-id="8d328-178">Esta coluna armazena valores de texto.</span><span class="sxs-lookup"><span data-stu-id="8d328-178">This column stores text values.</span></span>
| <span data-ttu-id="8d328-179">**isDeletable**</span><span class="sxs-lookup"><span data-stu-id="8d328-179">**isDeletable**</span></span>       | <span data-ttu-id="8d328-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d328-180">Boolean</span></span> | <span data-ttu-id="8d328-181">Indica se essa coluna pode ser excluída.</span><span class="sxs-lookup"><span data-stu-id="8d328-181">Indicates whether this column can be deleted.</span></span>
| <span data-ttu-id="8d328-182">**propagateChanges**</span><span class="sxs-lookup"><span data-stu-id="8d328-182">**propagateChanges**</span></span>     | <span data-ttu-id="8d328-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d328-183">Boolean</span></span> | <span data-ttu-id="8d328-184">Se as alterações 'True' nesta coluna serão propagadas para listas que implementam a coluna.</span><span class="sxs-lookup"><span data-stu-id="8d328-184">If 'True' changes to this column will be propagated to lists that implement the column.</span></span> 
| <span data-ttu-id="8d328-185">**isReorderable**</span><span class="sxs-lookup"><span data-stu-id="8d328-185">**isReorderable**</span></span>         | <span data-ttu-id="8d328-186">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d328-186">Boolean</span></span> | <span data-ttu-id="8d328-187">Indica se os valores na coluna podem ser reordenados.</span><span class="sxs-lookup"><span data-stu-id="8d328-187">Indicates whether values in the column can be reordered.</span></span> <span data-ttu-id="8d328-188">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8d328-188">Read-only.</span></span>
| <span data-ttu-id="8d328-189">**isSealed**</span><span class="sxs-lookup"><span data-stu-id="8d328-189">**isSealed**</span></span>              | <span data-ttu-id="8d328-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d328-190">Boolean</span></span> | <span data-ttu-id="8d328-191">Especifica se a coluna pode ser alterada.</span><span class="sxs-lookup"><span data-stu-id="8d328-191">Specifies whether column can be changed.</span></span>
| <span data-ttu-id="8d328-192">**validation**</span><span class="sxs-lookup"><span data-stu-id="8d328-192">**validation**</span></span>   |  <span data-ttu-id="8d328-193">[columnValidation][]</span><span class="sxs-lookup"><span data-stu-id="8d328-193">[columnValidation][]</span></span>    | <span data-ttu-id="8d328-194">Esta coluna armazena a fórmula e a mensagem de validação da coluna.</span><span class="sxs-lookup"><span data-stu-id="8d328-194">This column stores validation formula and message for the column.</span></span> 
| <span data-ttu-id="8d328-195">**hyperlinkOrPicture**</span><span class="sxs-lookup"><span data-stu-id="8d328-195">**hyperlinkOrPicture**</span></span>  | <span data-ttu-id="8d328-196">[hyperlinkOrPictureColumn][]</span><span class="sxs-lookup"><span data-stu-id="8d328-196">[hyperlinkOrPictureColumn][]</span></span> | <span data-ttu-id="8d328-197">Esta coluna armazena valores de hiperlink ou imagem.</span><span class="sxs-lookup"><span data-stu-id="8d328-197">This column stores hyperlink or picture values.</span></span> 
| <span data-ttu-id="8d328-198">**term**</span><span class="sxs-lookup"><span data-stu-id="8d328-198">**term**</span></span>     | <span data-ttu-id="8d328-199">[termColumn][]</span><span class="sxs-lookup"><span data-stu-id="8d328-199">[termColumn][]</span></span> | <span data-ttu-id="8d328-200">Esta coluna armazena termos de taxonomia.</span><span class="sxs-lookup"><span data-stu-id="8d328-200">This column stores taxonomy terms.</span></span>
| <span data-ttu-id="8d328-201">**sourceContentType**</span><span class="sxs-lookup"><span data-stu-id="8d328-201">**sourceContentType**</span></span>   |<span data-ttu-id="8d328-202">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="8d328-202">[contentTypeInfo][]</span></span>  | <span data-ttu-id="8d328-203">ContentType do qual esta coluna é herdada.</span><span class="sxs-lookup"><span data-stu-id="8d328-203">ContentType from which this column is inherited from.</span></span> <span data-ttu-id="8d328-204">Usado apenas ao buscar colunas contentTypes.</span><span class="sxs-lookup"><span data-stu-id="8d328-204">Used only while fetching contentTypes columns.</span></span>
| <span data-ttu-id="8d328-205">**thumbnail**</span><span class="sxs-lookup"><span data-stu-id="8d328-205">**thumbnail**</span></span>           |<span data-ttu-id="8d328-206">[thumbnailColumn][]</span><span class="sxs-lookup"><span data-stu-id="8d328-206">[thumbnailColumn][]</span></span>      | <span data-ttu-id="8d328-207">Esta coluna armazena valores de miniatura.</span><span class="sxs-lookup"><span data-stu-id="8d328-207">This column stores thumbnail values.</span></span>
| <span data-ttu-id="8d328-208">**tipo**</span><span class="sxs-lookup"><span data-stu-id="8d328-208">**type**</span></span>         | <span data-ttu-id="8d328-209">columnTypes</span><span class="sxs-lookup"><span data-stu-id="8d328-209">columnTypes</span></span>  | <span data-ttu-id="8d328-210">Para colunas de site, o tipo de coluna.</span><span class="sxs-lookup"><span data-stu-id="8d328-210">For site columns, the type of column.</span></span> <span data-ttu-id="8d328-211">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="8d328-211">Read-only</span></span>
| <span data-ttu-id="8d328-212">**contentApprovalStatus**</span><span class="sxs-lookup"><span data-stu-id="8d328-212">**contentApprovalStatus**</span></span>| <span data-ttu-id="8d328-213">[contentApprovalStatusColumn][]</span><span class="sxs-lookup"><span data-stu-id="8d328-213">[contentApprovalStatusColumn][]</span></span>     | <span data-ttu-id="8d328-214">Esta coluna armazena o status de aprovação de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="8d328-214">This column stores content approval status.</span></span>

## <a name="relationships"></a><span data-ttu-id="8d328-215">Relações</span><span class="sxs-lookup"><span data-stu-id="8d328-215">Relationships</span></span>

| <span data-ttu-id="8d328-216">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="8d328-216">Property name</span></span>   | <span data-ttu-id="8d328-217">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d328-217">Type</span></span>                      | <span data-ttu-id="8d328-218">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d328-218">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="8d328-219">**sourceColumn**</span><span class="sxs-lookup"><span data-stu-id="8d328-219">**sourceColumn**</span></span> | <span data-ttu-id="8d328-220">[columnDefinition][]</span><span class="sxs-lookup"><span data-stu-id="8d328-220">[columnDefinition][]</span></span> | <span data-ttu-id="8d328-221">A coluna de origem para a coluna de tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="8d328-221">The source column for content type column.</span></span>

><span data-ttu-id="8d328-222">**Observação:** Essas propriedades correspondem à enumeração [SPFieldType][] do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8d328-222">**Note:** These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="8d328-223">Embora os tipos de campo mais comuns sejam representados na tabela anterior, essa API beta ainda não tem alguns.</span><span class="sxs-lookup"><span data-stu-id="8d328-223">While the most common field types are represented in the previous table, this beta API is still missing some.</span></span>
<span data-ttu-id="8d328-224">nestes casos, nenhuma das facetas do tipo de coluna serão preenchidas, e a coluna só terá as propriedades básicas.</span><span class="sxs-lookup"><span data-stu-id="8d328-224">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="8d328-225">Comentários</span><span class="sxs-lookup"><span data-stu-id="8d328-225">Remarks</span></span>

<span data-ttu-id="8d328-226">Os valores ColumnDefinitions e valores de campo para colunas `hidden` não são mostrados por padrão.</span><span class="sxs-lookup"><span data-stu-id="8d328-226">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="8d328-227">Para vê-los ao listar **columnDefinitions**, inclua `hidden` na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="8d328-227">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="8d328-228">Para vê-los ao exibir valores **field** em [listItems][listItem], inclua as colunas desejadas por nome na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="8d328-228">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

[booleanColumn]: booleancolumn.md
[calculatedColumn]: calculatedcolumn.md
[choiceColumn]: choicecolumn.md
[columnDefinition]: columnDefinition.md
[currencyColumn]: currencycolumn.md
[dateTimeColumn]: datetimecolumn.md
[defaultColumnValue]: defaultcolumnvalue.md
[geolocationColumn]: geolocationcolumn.md
[lookupColumn]: lookupcolumn.md
[numberColumn]: numbercolumn.md
[personOrGroupColumn]: personorgroupcolumn.md
[textColumn]: textcolumn.md
[fieldValueSet]: fieldvalueset.md
[campos]: fieldvalueset.md
[fields]: fieldvalueset.md
[listItem]: listitem.md
[termColumn]: termColumn.md
[contentApprovalStatusColumn]: contentApprovalStatusColumn.md
[thumbnailColumn]: thumbnailColumn.md
[hyperlinkOrPictureColumn]: hyperlinkOrPictureColumn.md
[columnValidation]: columnValidation.md
[contentTypeInfo]: contentTypeInfo.md

<span data-ttu-id="8d328-249">
  [SPFieldType]: /previous-versions/office/sharepoint-server/ms428806(v=office.15)</span><span class="sxs-lookup"><span data-stu-id="8d328-249">[SPFieldType]: /previous-versions/office/sharepoint-server/ms428806(v=office.15)</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition",
  "suppressions": []
}
-->