---
author: JeremyKelley
description: Aqui está uma representação JSON de um recurso columnDefinition.
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: cddab6ee01cea34902ee892e593e0e81b3cde8af
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961297"
---
# <a name="columndefinition-resource-type"></a><span data-ttu-id="52768-103">Tipo de recurso columnDefinition</span><span class="sxs-lookup"><span data-stu-id="52768-103">columnDefinition resource type</span></span>

<span data-ttu-id="52768-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52768-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52768-105">Representa uma coluna em um [site,][] [lista][] ou [contentType][].</span><span class="sxs-lookup"><span data-stu-id="52768-105">Represents a column in a [site][], [list][] or [contentType][].</span></span>

## <a name="methods"></a><span data-ttu-id="52768-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="52768-106">Methods</span></span>
|<span data-ttu-id="52768-107">Método</span><span class="sxs-lookup"><span data-stu-id="52768-107">Method</span></span>|<span data-ttu-id="52768-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="52768-108">Return type</span></span>|<span data-ttu-id="52768-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="52768-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="52768-110">Listar colunas em um site</span><span class="sxs-lookup"><span data-stu-id="52768-110">List columns in a site</span></span>](../api/site-list-columns.md)|<span data-ttu-id="52768-111">[coleção columnDefinition](../resources/columndefinition.md)</span><span class="sxs-lookup"><span data-stu-id="52768-111">[columnDefinition](../resources/columndefinition.md) collection</span></span>|<span data-ttu-id="52768-112">Obter uma lista dos [objetos columnDefinition](../resources/columndefinition.md) e suas propriedades em um [site](../resources/site.md).</span><span class="sxs-lookup"><span data-stu-id="52768-112">Get a list of the [columnDefinition](../resources/columndefinition.md) objects and their properties in a [site](../resources/site.md).</span></span>|
|[<span data-ttu-id="52768-113">Listar colunas em uma lista</span><span class="sxs-lookup"><span data-stu-id="52768-113">List columns in a list</span></span>](../api/list-list-columns.md)|<span data-ttu-id="52768-114">[coleção columnDefinition](../resources/columndefinition.md)</span><span class="sxs-lookup"><span data-stu-id="52768-114">[columnDefinition](../resources/columndefinition.md) collection</span></span>|<span data-ttu-id="52768-115">Obter uma lista dos [objetos columnDefinition](../resources/columndefinition.md) e suas propriedades em uma [lista](../resources/list.md).</span><span class="sxs-lookup"><span data-stu-id="52768-115">Get a list of the [columnDefinition](../resources/columndefinition.md) objects and their properties in a [list](../resources/list.md).</span></span>|
|[<span data-ttu-id="52768-116">Listar colunas em um tipo de conteúdo</span><span class="sxs-lookup"><span data-stu-id="52768-116">List columns in a content type</span></span>](../api/contenttype-list-columns.md)|<span data-ttu-id="52768-117">[coleção columnDefinition](../resources/columndefinition.md)</span><span class="sxs-lookup"><span data-stu-id="52768-117">[columnDefinition](../resources/columndefinition.md) collection</span></span>|<span data-ttu-id="52768-118">Obter uma lista dos [objetos columnDefinition](../resources/columndefinition.md) e suas propriedades em um [tipo de conteúdo](../resources/contenttype.md).</span><span class="sxs-lookup"><span data-stu-id="52768-118">Get a list of the [columnDefinition](../resources/columndefinition.md) objects and their properties in a [content type](../resources/contenttype.md).</span></span>|
|[<span data-ttu-id="52768-119">Criar columnDefinition para um site</span><span class="sxs-lookup"><span data-stu-id="52768-119">Create columnDefinition for a site</span></span>](../api/site-post-columns.md)|[<span data-ttu-id="52768-120">columnDefinition</span><span class="sxs-lookup"><span data-stu-id="52768-120">columnDefinition</span></span>](../resources/columndefinition.md)|<span data-ttu-id="52768-121">Criar um novo [objeto columnDefinition](../resources/columndefinition.md) em um [site](../resources/site.md).</span><span class="sxs-lookup"><span data-stu-id="52768-121">Create a new [columnDefinition](../resources/columndefinition.md) object in a [site](../resources/site.md).</span></span>|
|[<span data-ttu-id="52768-122">Criar columnDefinition para uma lista</span><span class="sxs-lookup"><span data-stu-id="52768-122">Create columnDefinition for a list</span></span>](../api/list-post-columns.md)|[<span data-ttu-id="52768-123">columnDefinition</span><span class="sxs-lookup"><span data-stu-id="52768-123">columnDefinition</span></span>](../resources/columndefinition.md)|<span data-ttu-id="52768-124">Criar um novo [objeto columnDefinition](../resources/columndefinition.md) em uma [lista](../resources/list.md).</span><span class="sxs-lookup"><span data-stu-id="52768-124">Create a new [columnDefinition](../resources/columndefinition.md) object in a [list](../resources/list.md).</span></span>|
|[<span data-ttu-id="52768-125">Criar columnDefinition para um tipo de conteúdo</span><span class="sxs-lookup"><span data-stu-id="52768-125">Create columnDefinition for a content type</span></span>](../api/contenttype-post-columns.md)|[<span data-ttu-id="52768-126">columnDefinition</span><span class="sxs-lookup"><span data-stu-id="52768-126">columnDefinition</span></span>](../resources/columndefinition.md)|<span data-ttu-id="52768-127">Criar um novo [objeto columnDefinition](../resources/columndefinition.md) em um [tipo de conteúdo](../resources/contenttype.md).</span><span class="sxs-lookup"><span data-stu-id="52768-127">Create a new [columnDefinition](../resources/columndefinition.md) object in a [content type](../resources/contenttype.md).</span></span>|
|[<span data-ttu-id="52768-128">Obter columnDefinition</span><span class="sxs-lookup"><span data-stu-id="52768-128">Get columnDefinition</span></span>](../api/columndefinition-get.md)|[<span data-ttu-id="52768-129">columnDefinition</span><span class="sxs-lookup"><span data-stu-id="52768-129">columnDefinition</span></span>](../resources/columndefinition.md)|<span data-ttu-id="52768-130">Leia as propriedades e as relações de um [objeto columnDefinition.](../resources/columndefinition.md)</span><span class="sxs-lookup"><span data-stu-id="52768-130">Read the properties and relationships of a [columnDefinition](../resources/columndefinition.md) object.</span></span>|
|[<span data-ttu-id="52768-131">Atualizar columnDefinition</span><span class="sxs-lookup"><span data-stu-id="52768-131">Update columnDefinition</span></span>](../api/columndefinition-update.md)|[<span data-ttu-id="52768-132">columnDefinition</span><span class="sxs-lookup"><span data-stu-id="52768-132">columnDefinition</span></span>](../resources/columndefinition.md)|<span data-ttu-id="52768-133">Atualize as propriedades de um [objeto columnDefinition.](../resources/columndefinition.md)</span><span class="sxs-lookup"><span data-stu-id="52768-133">Update the properties of a [columnDefinition](../resources/columndefinition.md) object.</span></span>|
|[<span data-ttu-id="52768-134">Excluir columnDefinition</span><span class="sxs-lookup"><span data-stu-id="52768-134">Delete columnDefinition</span></span>](../api/columndefinition-delete.md)|<span data-ttu-id="52768-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="52768-135">None</span></span>|<span data-ttu-id="52768-136">Exclui um [objeto columnDefinition.](../resources/columndefinition.md)</span><span class="sxs-lookup"><span data-stu-id="52768-136">Deletes a [columnDefinition](../resources/columndefinition.md) object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="52768-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52768-137">JSON representation</span></span>

<span data-ttu-id="52768-138">Aqui está uma representação JSON de um recurso columnDefinition.</span><span class="sxs-lookup"><span data-stu-id="52768-138">Here is a JSON representation of a columnDefinition resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="52768-139">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52768-139">Properties</span></span>

<span data-ttu-id="52768-140">As colunas podem conter dados de vários tipos.</span><span class="sxs-lookup"><span data-stu-id="52768-140">Columns can hold data of various types.</span></span>
<span data-ttu-id="52768-141">As propriedades a seguir indicam qual tipo de dados uma coluna armazena, bem como configurações adicionais para esses dados.</span><span class="sxs-lookup"><span data-stu-id="52768-141">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="52768-142">As propriedades relacionadas ao tipo (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) são mutuamente exclusivas. Uma coluna só pode ter uma delas especificada.</span><span class="sxs-lookup"><span data-stu-id="52768-142">The type-related properties (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="52768-143">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="52768-143">Property name</span></span>           | <span data-ttu-id="52768-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="52768-144">Type</span></span>    | <span data-ttu-id="52768-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="52768-145">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="52768-146">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="52768-146">**columnGroup**</span></span>         | <span data-ttu-id="52768-147">string</span><span class="sxs-lookup"><span data-stu-id="52768-147">string</span></span>  | <span data-ttu-id="52768-148">Para colunas de site, o nome do grupo ao qual esta coluna pertence.</span><span class="sxs-lookup"><span data-stu-id="52768-148">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="52768-149">Ajuda a organizar as colunas relacionadas.</span><span class="sxs-lookup"><span data-stu-id="52768-149">Helps organize related columns.</span></span>
| <span data-ttu-id="52768-150">**description**</span><span class="sxs-lookup"><span data-stu-id="52768-150">**description**</span></span>         | <span data-ttu-id="52768-151">string</span><span class="sxs-lookup"><span data-stu-id="52768-151">string</span></span>  | <span data-ttu-id="52768-152">A descrição voltado para o usuário da coluna.</span><span class="sxs-lookup"><span data-stu-id="52768-152">The user-facing description of the column.</span></span>
| <span data-ttu-id="52768-153">**displayName**</span><span class="sxs-lookup"><span data-stu-id="52768-153">**displayName**</span></span>         | <span data-ttu-id="52768-154">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52768-154">string</span></span>  | <span data-ttu-id="52768-155">O nome voltado para o usuário da coluna.</span><span class="sxs-lookup"><span data-stu-id="52768-155">The user-facing name of the column.</span></span>
| <span data-ttu-id="52768-156">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="52768-156">**enforceUniqueValues**</span></span> | <span data-ttu-id="52768-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="52768-157">Boolean</span></span> | <span data-ttu-id="52768-158">Se for verdadeiro, esse mesmo valor não constará em dois itens de lista nessa coluna.</span><span class="sxs-lookup"><span data-stu-id="52768-158">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="52768-159">**hidden**</span><span class="sxs-lookup"><span data-stu-id="52768-159">**hidden**</span></span>              | <span data-ttu-id="52768-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="52768-160">Boolean</span></span> | <span data-ttu-id="52768-161">Especifica se a coluna é exibida na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="52768-161">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="52768-162">**id**</span><span class="sxs-lookup"><span data-stu-id="52768-162">**id**</span></span>                  | <span data-ttu-id="52768-163">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52768-163">string</span></span>  | <span data-ttu-id="52768-164">O identificador exclusivo da coluna.</span><span class="sxs-lookup"><span data-stu-id="52768-164">The unique identifier for the column.</span></span>
| <span data-ttu-id="52768-165">**indexed**</span><span class="sxs-lookup"><span data-stu-id="52768-165">**indexed**</span></span>             | <span data-ttu-id="52768-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="52768-166">Boolean</span></span> | <span data-ttu-id="52768-167">Especifica se os valores da coluna podem ser usados para classificação e pesquisa.</span><span class="sxs-lookup"><span data-stu-id="52768-167">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="52768-168">**name**</span><span class="sxs-lookup"><span data-stu-id="52768-168">**name**</span></span>                | <span data-ttu-id="52768-169">string</span><span class="sxs-lookup"><span data-stu-id="52768-169">string</span></span>  | <span data-ttu-id="52768-170">O nome voltado para a API da coluna, conforme ele aparece nos [campos][] em uma [listItem][].</span><span class="sxs-lookup"><span data-stu-id="52768-170">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="52768-171">Para o nome voltado ao usuário, consulte **displayName**.</span><span class="sxs-lookup"><span data-stu-id="52768-171">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="52768-172">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="52768-172">**readOnly**</span></span>            | <span data-ttu-id="52768-173">Booliano</span><span class="sxs-lookup"><span data-stu-id="52768-173">Boolean</span></span>    | <span data-ttu-id="52768-174">Especifica se os valores da coluna podem ser modificados.</span><span class="sxs-lookup"><span data-stu-id="52768-174">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="52768-175">**required**</span><span class="sxs-lookup"><span data-stu-id="52768-175">**required**</span></span>            | <span data-ttu-id="52768-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="52768-176">Boolean</span></span> | <span data-ttu-id="52768-177">Especifica se o valor da coluna não é opcional.</span><span class="sxs-lookup"><span data-stu-id="52768-177">Specifies whether the column value is not optional.</span></span>
| <span data-ttu-id="52768-178">**boolean**</span><span class="sxs-lookup"><span data-stu-id="52768-178">**boolean**</span></span>       | <span data-ttu-id="52768-179">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="52768-179">[booleanColumn][]</span></span>       | <span data-ttu-id="52768-180">Esta coluna armazena valores boolianos.</span><span class="sxs-lookup"><span data-stu-id="52768-180">This column stores boolean values.</span></span>
| <span data-ttu-id="52768-181">**calculated**</span><span class="sxs-lookup"><span data-stu-id="52768-181">**calculated**</span></span>    | <span data-ttu-id="52768-182">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="52768-182">[calculatedColumn][]</span></span>    | <span data-ttu-id="52768-183">Os dados dessa coluna são calculados com base em outras colunas.</span><span class="sxs-lookup"><span data-stu-id="52768-183">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="52768-184">**choice**</span><span class="sxs-lookup"><span data-stu-id="52768-184">**choice**</span></span>        | <span data-ttu-id="52768-185">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="52768-185">[choiceColumn][]</span></span>        | <span data-ttu-id="52768-186">Esta coluna armazena dados de uma lista de opções.</span><span class="sxs-lookup"><span data-stu-id="52768-186">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="52768-187">**currency**</span><span class="sxs-lookup"><span data-stu-id="52768-187">**currency**</span></span>      | <span data-ttu-id="52768-188">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="52768-188">[currencyColumn][]</span></span>      | <span data-ttu-id="52768-189">Esta coluna armazena valores monetários.</span><span class="sxs-lookup"><span data-stu-id="52768-189">This column stores currency values.</span></span>
| <span data-ttu-id="52768-190">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="52768-190">**dateTime**</span></span>      | <span data-ttu-id="52768-191">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="52768-191">[dateTimeColumn][]</span></span>      | <span data-ttu-id="52768-192">Esta coluna armazena valores de datetime.</span><span class="sxs-lookup"><span data-stu-id="52768-192">This column stores DateTime values.</span></span>
| <span data-ttu-id="52768-193">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="52768-193">**defaultValue**</span></span>  | <span data-ttu-id="52768-194">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="52768-194">[defaultColumnValue][]</span></span>  | <span data-ttu-id="52768-195">O valor padrão dessa coluna.</span><span class="sxs-lookup"><span data-stu-id="52768-195">The default value for this column.</span></span>
| <span data-ttu-id="52768-196">**geolocalização**</span><span class="sxs-lookup"><span data-stu-id="52768-196">**geolocation**</span></span>   | <span data-ttu-id="52768-197">[geolocationColumn][]</span><span class="sxs-lookup"><span data-stu-id="52768-197">[geolocationColumn][]</span></span>   | <span data-ttu-id="52768-198">Esta coluna armazena uma localização geográfica.</span><span class="sxs-lookup"><span data-stu-id="52768-198">This column stores a geolocation.</span></span>
| <span data-ttu-id="52768-199">**lookup**</span><span class="sxs-lookup"><span data-stu-id="52768-199">**lookup**</span></span>        | <span data-ttu-id="52768-200">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="52768-200">[lookupColumn][]</span></span>        | <span data-ttu-id="52768-201">Os dados dessa coluna são procurados por outra fonte no site.</span><span class="sxs-lookup"><span data-stu-id="52768-201">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="52768-202">**number**</span><span class="sxs-lookup"><span data-stu-id="52768-202">**number**</span></span>        | <span data-ttu-id="52768-203">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="52768-203">[numberColumn][]</span></span>        | <span data-ttu-id="52768-204">Esta coluna armazena valores numéricos.</span><span class="sxs-lookup"><span data-stu-id="52768-204">This column stores number values.</span></span>
| <span data-ttu-id="52768-205">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="52768-205">**personOrGroup**</span></span> | <span data-ttu-id="52768-206">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="52768-206">[personOrGroupColumn][]</span></span> | <span data-ttu-id="52768-207">Esta coluna armazena valores de Pessoa ou Grupo.</span><span class="sxs-lookup"><span data-stu-id="52768-207">This column stores Person or Group values.</span></span>
| <span data-ttu-id="52768-208">**text**</span><span class="sxs-lookup"><span data-stu-id="52768-208">**text**</span></span>          | <span data-ttu-id="52768-209">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="52768-209">[textColumn][]</span></span>          | <span data-ttu-id="52768-210">Esta coluna armazena valores de texto.</span><span class="sxs-lookup"><span data-stu-id="52768-210">This column stores text values.</span></span>
| <span data-ttu-id="52768-211">**isDeletable**</span><span class="sxs-lookup"><span data-stu-id="52768-211">**isDeletable**</span></span>       | <span data-ttu-id="52768-212">Booliano</span><span class="sxs-lookup"><span data-stu-id="52768-212">Boolean</span></span> | <span data-ttu-id="52768-213">Indica se essa coluna pode ser excluída.</span><span class="sxs-lookup"><span data-stu-id="52768-213">Indicates whether this column can be deleted.</span></span>
| <span data-ttu-id="52768-214">**propagateChanges**</span><span class="sxs-lookup"><span data-stu-id="52768-214">**propagateChanges**</span></span>     | <span data-ttu-id="52768-215">Booliano</span><span class="sxs-lookup"><span data-stu-id="52768-215">Boolean</span></span> | <span data-ttu-id="52768-216">Se as alterações 'True' nesta coluna serão propagadas para listas que implementam a coluna.</span><span class="sxs-lookup"><span data-stu-id="52768-216">If 'True' changes to this column will be propagated to lists that implement the column.</span></span> 
| <span data-ttu-id="52768-217">**isReorderable**</span><span class="sxs-lookup"><span data-stu-id="52768-217">**isReorderable**</span></span>         | <span data-ttu-id="52768-218">Booliano</span><span class="sxs-lookup"><span data-stu-id="52768-218">Boolean</span></span> | <span data-ttu-id="52768-219">Indica se os valores na coluna podem ser reordenados.</span><span class="sxs-lookup"><span data-stu-id="52768-219">Indicates whether values in the column can be reordered.</span></span> <span data-ttu-id="52768-220">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52768-220">Read-only.</span></span>
| <span data-ttu-id="52768-221">**isSealed**</span><span class="sxs-lookup"><span data-stu-id="52768-221">**isSealed**</span></span>              | <span data-ttu-id="52768-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="52768-222">Boolean</span></span> | <span data-ttu-id="52768-223">Especifica se a coluna pode ser alterada.</span><span class="sxs-lookup"><span data-stu-id="52768-223">Specifies whether column can be changed.</span></span>
| <span data-ttu-id="52768-224">**validation**</span><span class="sxs-lookup"><span data-stu-id="52768-224">**validation**</span></span>   |  <span data-ttu-id="52768-225">[columnValidation][]</span><span class="sxs-lookup"><span data-stu-id="52768-225">[columnValidation][]</span></span>    | <span data-ttu-id="52768-226">Esta coluna armazena a fórmula e a mensagem de validação da coluna.</span><span class="sxs-lookup"><span data-stu-id="52768-226">This column stores validation formula and message for the column.</span></span> 
| <span data-ttu-id="52768-227">**hyperlinkOrPicture**</span><span class="sxs-lookup"><span data-stu-id="52768-227">**hyperlinkOrPicture**</span></span>  | <span data-ttu-id="52768-228">[hyperlinkOrPictureColumn][]</span><span class="sxs-lookup"><span data-stu-id="52768-228">[hyperlinkOrPictureColumn][]</span></span> | <span data-ttu-id="52768-229">Esta coluna armazena valores de hiperlink ou imagem.</span><span class="sxs-lookup"><span data-stu-id="52768-229">This column stores hyperlink or picture values.</span></span> 
| <span data-ttu-id="52768-230">**term**</span><span class="sxs-lookup"><span data-stu-id="52768-230">**term**</span></span>     | <span data-ttu-id="52768-231">[termColumn][]</span><span class="sxs-lookup"><span data-stu-id="52768-231">[termColumn][]</span></span> | <span data-ttu-id="52768-232">Esta coluna armazena termos de taxonomia.</span><span class="sxs-lookup"><span data-stu-id="52768-232">This column stores taxonomy terms.</span></span>
| <span data-ttu-id="52768-233">**sourceContentType**</span><span class="sxs-lookup"><span data-stu-id="52768-233">**sourceContentType**</span></span>   |<span data-ttu-id="52768-234">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="52768-234">[contentTypeInfo][]</span></span>  | <span data-ttu-id="52768-235">ContentType do qual esta coluna é herdada.</span><span class="sxs-lookup"><span data-stu-id="52768-235">ContentType from which this column is inherited from.</span></span> <span data-ttu-id="52768-236">Usado apenas ao buscar colunas contentTypes.</span><span class="sxs-lookup"><span data-stu-id="52768-236">Used only while fetching contentTypes columns.</span></span>
| <span data-ttu-id="52768-237">**thumbnail**</span><span class="sxs-lookup"><span data-stu-id="52768-237">**thumbnail**</span></span>           |<span data-ttu-id="52768-238">[thumbnailColumn][]</span><span class="sxs-lookup"><span data-stu-id="52768-238">[thumbnailColumn][]</span></span>      | <span data-ttu-id="52768-239">Esta coluna armazena valores de miniatura.</span><span class="sxs-lookup"><span data-stu-id="52768-239">This column stores thumbnail values.</span></span>
| <span data-ttu-id="52768-240">**type**</span><span class="sxs-lookup"><span data-stu-id="52768-240">**type**</span></span>         | <span data-ttu-id="52768-241">columnTypes</span><span class="sxs-lookup"><span data-stu-id="52768-241">columnTypes</span></span>  | <span data-ttu-id="52768-242">Para colunas de site, o tipo de coluna.</span><span class="sxs-lookup"><span data-stu-id="52768-242">For site columns, the type of column.</span></span> <span data-ttu-id="52768-243">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="52768-243">Read-only</span></span>
| <span data-ttu-id="52768-244">**contentApprovalStatus**</span><span class="sxs-lookup"><span data-stu-id="52768-244">**contentApprovalStatus**</span></span>| <span data-ttu-id="52768-245">[contentApprovalStatusColumn][]</span><span class="sxs-lookup"><span data-stu-id="52768-245">[contentApprovalStatusColumn][]</span></span>     | <span data-ttu-id="52768-246">Esta coluna armazena o status de aprovação de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="52768-246">This column stores content approval status.</span></span>

## <a name="relationships"></a><span data-ttu-id="52768-247">Relações</span><span class="sxs-lookup"><span data-stu-id="52768-247">Relationships</span></span>

| <span data-ttu-id="52768-248">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="52768-248">Property name</span></span>   | <span data-ttu-id="52768-249">Tipo</span><span class="sxs-lookup"><span data-stu-id="52768-249">Type</span></span>                      | <span data-ttu-id="52768-250">Descrição</span><span class="sxs-lookup"><span data-stu-id="52768-250">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="52768-251">**sourceColumn**</span><span class="sxs-lookup"><span data-stu-id="52768-251">**sourceColumn**</span></span> | <span data-ttu-id="52768-252">[columnDefinition][]</span><span class="sxs-lookup"><span data-stu-id="52768-252">[columnDefinition][]</span></span> | <span data-ttu-id="52768-253">A coluna de origem para a coluna de tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="52768-253">The source column for content type column.</span></span>

><span data-ttu-id="52768-254">**Observação:** Essas propriedades correspondem à enumeração [SPFieldType][] do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="52768-254">**Note:** These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="52768-255">Embora os tipos de campo mais comuns sejam representados na tabela anterior, essa API beta ainda não tem alguns.</span><span class="sxs-lookup"><span data-stu-id="52768-255">While the most common field types are represented in the previous table, this beta API is still missing some.</span></span>
<span data-ttu-id="52768-256">nestes casos, nenhuma das facetas do tipo de coluna serão preenchidas, e a coluna só terá as propriedades básicas.</span><span class="sxs-lookup"><span data-stu-id="52768-256">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="52768-257">Comentários</span><span class="sxs-lookup"><span data-stu-id="52768-257">Remarks</span></span>

<span data-ttu-id="52768-258">Os valores ColumnDefinitions e valores de campo para colunas `hidden` não são mostrados por padrão.</span><span class="sxs-lookup"><span data-stu-id="52768-258">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="52768-259">Para vê-los ao listar **columnDefinitions**, inclua `hidden` na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="52768-259">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="52768-260">Para vê-los ao exibir valores **field** em [listItems][listItem], inclua as colunas desejadas por nome na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="52768-260">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

[booleanColumn]: booleancolumn.md
[calculatedColumn]: calculatedcolumn.md
[choiceColumn]: choicecolumn.md
[columnDefinition]: columnDefinition.md
[contentType]: contenttype.md
[currencyColumn]: currencycolumn.md
[dateTimeColumn]: datetimecolumn.md
[defaultColumnValue]: defaultcolumnvalue.md
[geolocationColumn]: geolocationcolumn.md
[list]: list.md
[lookupColumn]: lookupcolumn.md
[numberColumn]: numbercolumn.md
[personOrGroupColumn]: personorgroupcolumn.md
[site]: site.md
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

<span data-ttu-id="52768-284">
  [SPFieldType]: /previous-versions/office/sharepoint-server/ms428806(v=office.15)</span><span class="sxs-lookup"><span data-stu-id="52768-284">[SPFieldType]: /previous-versions/office/sharepoint-server/ms428806(v=office.15)</span></span>

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