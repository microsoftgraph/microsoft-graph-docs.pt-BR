---
author: JeremyKelley
description: Representa uma coluna em um site, uma lista ou um contentType.
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 982b9751f522d34a5cdf1dd329262486d35bfb0a
ms.sourcegitcommit: 73bbf84e6f5dbc8c3db8ed2c48cc5ab9ae3cff78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2021
ms.locfileid: "53456468"
---
# <a name="columndefinition-resource-type"></a><span data-ttu-id="62fa1-103">Tipo de recurso columnDefinition</span><span class="sxs-lookup"><span data-stu-id="62fa1-103">columnDefinition resource type</span></span>

<span data-ttu-id="62fa1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62fa1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62fa1-105">Representa uma coluna em um [site,][] [lista][] ou [contentType][].</span><span class="sxs-lookup"><span data-stu-id="62fa1-105">Represents a column in a [site][], [list][] or [contentType][].</span></span>

## <a name="methods"></a><span data-ttu-id="62fa1-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="62fa1-106">Methods</span></span>
|<span data-ttu-id="62fa1-107">Método</span><span class="sxs-lookup"><span data-stu-id="62fa1-107">Method</span></span>|<span data-ttu-id="62fa1-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="62fa1-108">Return type</span></span>|<span data-ttu-id="62fa1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="62fa1-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="62fa1-110">Listar colunas em um site</span><span class="sxs-lookup"><span data-stu-id="62fa1-110">List columns in a site</span></span>](../api/site-list-columns.md)|<span data-ttu-id="62fa1-111">[coleção columnDefinition](../resources/columndefinition.md)</span><span class="sxs-lookup"><span data-stu-id="62fa1-111">[columnDefinition](../resources/columndefinition.md) collection</span></span>|<span data-ttu-id="62fa1-112">Obter uma lista dos [objetos columnDefinition](../resources/columndefinition.md) e suas propriedades em um [site](../resources/site.md).</span><span class="sxs-lookup"><span data-stu-id="62fa1-112">Get a list of the [columnDefinition](../resources/columndefinition.md) objects and their properties in a [site](../resources/site.md).</span></span>|
|[<span data-ttu-id="62fa1-113">Listar colunas em uma lista</span><span class="sxs-lookup"><span data-stu-id="62fa1-113">List columns in a list</span></span>](../api/list-list-columns.md)|<span data-ttu-id="62fa1-114">[coleção columnDefinition](../resources/columndefinition.md)</span><span class="sxs-lookup"><span data-stu-id="62fa1-114">[columnDefinition](../resources/columndefinition.md) collection</span></span>|<span data-ttu-id="62fa1-115">Obter uma lista dos [objetos columnDefinition](../resources/columndefinition.md) e suas propriedades em uma [lista](../resources/list.md).</span><span class="sxs-lookup"><span data-stu-id="62fa1-115">Get a list of the [columnDefinition](../resources/columndefinition.md) objects and their properties in a [list](../resources/list.md).</span></span>|
|[<span data-ttu-id="62fa1-116">Listar colunas em um tipo de conteúdo</span><span class="sxs-lookup"><span data-stu-id="62fa1-116">List columns in a content type</span></span>](../api/contenttype-list-columns.md)|<span data-ttu-id="62fa1-117">[coleção columnDefinition](../resources/columndefinition.md)</span><span class="sxs-lookup"><span data-stu-id="62fa1-117">[columnDefinition](../resources/columndefinition.md) collection</span></span>|<span data-ttu-id="62fa1-118">Obter uma lista dos [objetos columnDefinition](../resources/columndefinition.md) e suas propriedades em um [tipo de conteúdo](../resources/contenttype.md).</span><span class="sxs-lookup"><span data-stu-id="62fa1-118">Get a list of the [columnDefinition](../resources/columndefinition.md) objects and their properties in a [content type](../resources/contenttype.md).</span></span>|
|[<span data-ttu-id="62fa1-119">Criar columnDefinition para um site</span><span class="sxs-lookup"><span data-stu-id="62fa1-119">Create columnDefinition for a site</span></span>](../api/site-post-columns.md)|[<span data-ttu-id="62fa1-120">columnDefinition</span><span class="sxs-lookup"><span data-stu-id="62fa1-120">columnDefinition</span></span>](../resources/columndefinition.md)|<span data-ttu-id="62fa1-121">Criar um novo [objeto columnDefinition](../resources/columndefinition.md) em um [site](../resources/site.md).</span><span class="sxs-lookup"><span data-stu-id="62fa1-121">Create a new [columnDefinition](../resources/columndefinition.md) object in a [site](../resources/site.md).</span></span>|
|[<span data-ttu-id="62fa1-122">Criar columnDefinition para uma lista</span><span class="sxs-lookup"><span data-stu-id="62fa1-122">Create columnDefinition for a list</span></span>](../api/list-post-columns.md)|[<span data-ttu-id="62fa1-123">columnDefinition</span><span class="sxs-lookup"><span data-stu-id="62fa1-123">columnDefinition</span></span>](../resources/columndefinition.md)|<span data-ttu-id="62fa1-124">Criar um novo [objeto columnDefinition](../resources/columndefinition.md) em uma [lista](../resources/list.md).</span><span class="sxs-lookup"><span data-stu-id="62fa1-124">Create a new [columnDefinition](../resources/columndefinition.md) object in a [list](../resources/list.md).</span></span>|
|[<span data-ttu-id="62fa1-125">Criar columnDefinition para um tipo de conteúdo</span><span class="sxs-lookup"><span data-stu-id="62fa1-125">Create columnDefinition for a content type</span></span>](../api/contenttype-post-columns.md)|[<span data-ttu-id="62fa1-126">columnDefinition</span><span class="sxs-lookup"><span data-stu-id="62fa1-126">columnDefinition</span></span>](../resources/columndefinition.md)|<span data-ttu-id="62fa1-127">Criar um novo [objeto columnDefinition](../resources/columndefinition.md) em um [tipo de conteúdo](../resources/contenttype.md).</span><span class="sxs-lookup"><span data-stu-id="62fa1-127">Create a new [columnDefinition](../resources/columndefinition.md) object in a [content type](../resources/contenttype.md).</span></span>|
|[<span data-ttu-id="62fa1-128">Obter columnDefinition</span><span class="sxs-lookup"><span data-stu-id="62fa1-128">Get columnDefinition</span></span>](../api/columndefinition-get.md)|[<span data-ttu-id="62fa1-129">columnDefinition</span><span class="sxs-lookup"><span data-stu-id="62fa1-129">columnDefinition</span></span>](../resources/columndefinition.md)|<span data-ttu-id="62fa1-130">Leia as propriedades e as relações de um [objeto columnDefinition.](../resources/columndefinition.md)</span><span class="sxs-lookup"><span data-stu-id="62fa1-130">Read the properties and relationships of a [columnDefinition](../resources/columndefinition.md) object.</span></span>|
|[<span data-ttu-id="62fa1-131">Atualizar columnDefinition</span><span class="sxs-lookup"><span data-stu-id="62fa1-131">Update columnDefinition</span></span>](../api/columndefinition-update.md)|[<span data-ttu-id="62fa1-132">columnDefinition</span><span class="sxs-lookup"><span data-stu-id="62fa1-132">columnDefinition</span></span>](../resources/columndefinition.md)|<span data-ttu-id="62fa1-133">Atualize as propriedades de um [objeto columnDefinition.](../resources/columndefinition.md)</span><span class="sxs-lookup"><span data-stu-id="62fa1-133">Update the properties of a [columnDefinition](../resources/columndefinition.md) object.</span></span>|
|[<span data-ttu-id="62fa1-134">Excluir columnDefinition</span><span class="sxs-lookup"><span data-stu-id="62fa1-134">Delete columnDefinition</span></span>](../api/columndefinition-delete.md)|<span data-ttu-id="62fa1-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="62fa1-135">None</span></span>|<span data-ttu-id="62fa1-136">Exclui um [objeto columnDefinition.](../resources/columndefinition.md)</span><span class="sxs-lookup"><span data-stu-id="62fa1-136">Deletes a [columnDefinition](../resources/columndefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="62fa1-137">Propriedades</span><span class="sxs-lookup"><span data-stu-id="62fa1-137">Properties</span></span>

<span data-ttu-id="62fa1-138">As colunas podem conter dados de vários tipos.</span><span class="sxs-lookup"><span data-stu-id="62fa1-138">Columns can hold data of various types.</span></span>
<span data-ttu-id="62fa1-139">As propriedades a seguir indicam qual tipo de dados uma coluna armazena, bem como configurações adicionais para esses dados.</span><span class="sxs-lookup"><span data-stu-id="62fa1-139">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="62fa1-140">As propriedades relacionadas ao tipo (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) são mutuamente exclusivas. Uma coluna só pode ter uma delas especificada.</span><span class="sxs-lookup"><span data-stu-id="62fa1-140">The type-related properties (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="62fa1-141">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="62fa1-141">Property name</span></span>           | <span data-ttu-id="62fa1-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="62fa1-142">Type</span></span>    | <span data-ttu-id="62fa1-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="62fa1-143">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="62fa1-144">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="62fa1-144">**columnGroup**</span></span>         | <span data-ttu-id="62fa1-145">string</span><span class="sxs-lookup"><span data-stu-id="62fa1-145">string</span></span>  | <span data-ttu-id="62fa1-146">Para colunas de site, o nome do grupo ao qual esta coluna pertence.</span><span class="sxs-lookup"><span data-stu-id="62fa1-146">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="62fa1-147">Ajuda a organizar as colunas relacionadas.</span><span class="sxs-lookup"><span data-stu-id="62fa1-147">Helps organize related columns.</span></span>
| <span data-ttu-id="62fa1-148">**description**</span><span class="sxs-lookup"><span data-stu-id="62fa1-148">**description**</span></span>         | <span data-ttu-id="62fa1-149">string</span><span class="sxs-lookup"><span data-stu-id="62fa1-149">string</span></span>  | <span data-ttu-id="62fa1-150">A descrição voltado para o usuário da coluna.</span><span class="sxs-lookup"><span data-stu-id="62fa1-150">The user-facing description of the column.</span></span>
| <span data-ttu-id="62fa1-151">**displayName**</span><span class="sxs-lookup"><span data-stu-id="62fa1-151">**displayName**</span></span>         | <span data-ttu-id="62fa1-152">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62fa1-152">string</span></span>  | <span data-ttu-id="62fa1-153">O nome voltado para o usuário da coluna.</span><span class="sxs-lookup"><span data-stu-id="62fa1-153">The user-facing name of the column.</span></span>
| <span data-ttu-id="62fa1-154">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="62fa1-154">**enforceUniqueValues**</span></span> | <span data-ttu-id="62fa1-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="62fa1-155">Boolean</span></span> | <span data-ttu-id="62fa1-156">If `true` , no two list items may have the same value for this column.</span><span class="sxs-lookup"><span data-stu-id="62fa1-156">If `true`, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="62fa1-157">**hidden**</span><span class="sxs-lookup"><span data-stu-id="62fa1-157">**hidden**</span></span>              | <span data-ttu-id="62fa1-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="62fa1-158">Boolean</span></span> | <span data-ttu-id="62fa1-159">Especifica se a coluna é exibida na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="62fa1-159">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="62fa1-160">**id**</span><span class="sxs-lookup"><span data-stu-id="62fa1-160">**id**</span></span>                  | <span data-ttu-id="62fa1-161">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62fa1-161">string</span></span>  | <span data-ttu-id="62fa1-162">O identificador exclusivo da coluna.</span><span class="sxs-lookup"><span data-stu-id="62fa1-162">The unique identifier for the column.</span></span>
| <span data-ttu-id="62fa1-163">**indexed**</span><span class="sxs-lookup"><span data-stu-id="62fa1-163">**indexed**</span></span>             | <span data-ttu-id="62fa1-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="62fa1-164">Boolean</span></span> | <span data-ttu-id="62fa1-165">Especifica se os valores da coluna podem ser usados para classificação e pesquisa.</span><span class="sxs-lookup"><span data-stu-id="62fa1-165">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="62fa1-166">**name**</span><span class="sxs-lookup"><span data-stu-id="62fa1-166">**name**</span></span>                | <span data-ttu-id="62fa1-167">string</span><span class="sxs-lookup"><span data-stu-id="62fa1-167">string</span></span>  | <span data-ttu-id="62fa1-168">O nome voltado para a API da coluna, conforme ele aparece nos [campos][] em uma [listItem][].</span><span class="sxs-lookup"><span data-stu-id="62fa1-168">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="62fa1-169">Para o nome voltado ao usuário, consulte **displayName**.</span><span class="sxs-lookup"><span data-stu-id="62fa1-169">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="62fa1-170">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="62fa1-170">**readOnly**</span></span>            | <span data-ttu-id="62fa1-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="62fa1-171">Boolean</span></span>    | <span data-ttu-id="62fa1-172">Especifica se os valores da coluna podem ser modificados.</span><span class="sxs-lookup"><span data-stu-id="62fa1-172">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="62fa1-173">**required**</span><span class="sxs-lookup"><span data-stu-id="62fa1-173">**required**</span></span>            | <span data-ttu-id="62fa1-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="62fa1-174">Boolean</span></span> | <span data-ttu-id="62fa1-175">Especifica se o valor da coluna não é opcional.</span><span class="sxs-lookup"><span data-stu-id="62fa1-175">Specifies whether the column value isn't optional.</span></span>
| <span data-ttu-id="62fa1-176">**boolean**</span><span class="sxs-lookup"><span data-stu-id="62fa1-176">**boolean**</span></span>       | <span data-ttu-id="62fa1-177">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="62fa1-177">[booleanColumn][]</span></span>       | <span data-ttu-id="62fa1-178">Esta coluna armazena valores boolianos.</span><span class="sxs-lookup"><span data-stu-id="62fa1-178">This column stores boolean values.</span></span>
| <span data-ttu-id="62fa1-179">**calculated**</span><span class="sxs-lookup"><span data-stu-id="62fa1-179">**calculated**</span></span>    | <span data-ttu-id="62fa1-180">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="62fa1-180">[calculatedColumn][]</span></span>    | <span data-ttu-id="62fa1-181">Os dados dessa coluna são calculados com base em outras colunas.</span><span class="sxs-lookup"><span data-stu-id="62fa1-181">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="62fa1-182">**choice**</span><span class="sxs-lookup"><span data-stu-id="62fa1-182">**choice**</span></span>        | <span data-ttu-id="62fa1-183">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="62fa1-183">[choiceColumn][]</span></span>        | <span data-ttu-id="62fa1-184">Esta coluna armazena dados de uma lista de opções.</span><span class="sxs-lookup"><span data-stu-id="62fa1-184">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="62fa1-185">**currency**</span><span class="sxs-lookup"><span data-stu-id="62fa1-185">**currency**</span></span>      | <span data-ttu-id="62fa1-186">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="62fa1-186">[currencyColumn][]</span></span>      | <span data-ttu-id="62fa1-187">Esta coluna armazena valores monetários.</span><span class="sxs-lookup"><span data-stu-id="62fa1-187">This column stores currency values.</span></span>
| <span data-ttu-id="62fa1-188">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="62fa1-188">**dateTime**</span></span>      | <span data-ttu-id="62fa1-189">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="62fa1-189">[dateTimeColumn][]</span></span>      | <span data-ttu-id="62fa1-190">Esta coluna armazena valores de datetime.</span><span class="sxs-lookup"><span data-stu-id="62fa1-190">This column stores DateTime values.</span></span>
| <span data-ttu-id="62fa1-191">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="62fa1-191">**defaultValue**</span></span>  | <span data-ttu-id="62fa1-192">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="62fa1-192">[defaultColumnValue][]</span></span>  | <span data-ttu-id="62fa1-193">O valor padrão dessa coluna.</span><span class="sxs-lookup"><span data-stu-id="62fa1-193">The default value for this column.</span></span>
| <span data-ttu-id="62fa1-194">**geolocalização**</span><span class="sxs-lookup"><span data-stu-id="62fa1-194">**geolocation**</span></span>   | <span data-ttu-id="62fa1-195">[geolocationColumn][]</span><span class="sxs-lookup"><span data-stu-id="62fa1-195">[geolocationColumn][]</span></span>   | <span data-ttu-id="62fa1-196">Esta coluna armazena uma localização geográfica.</span><span class="sxs-lookup"><span data-stu-id="62fa1-196">This column stores a geolocation.</span></span>
| <span data-ttu-id="62fa1-197">**lookup**</span><span class="sxs-lookup"><span data-stu-id="62fa1-197">**lookup**</span></span>        | <span data-ttu-id="62fa1-198">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="62fa1-198">[lookupColumn][]</span></span>        | <span data-ttu-id="62fa1-199">Os dados dessa coluna são procurados por outra fonte no site.</span><span class="sxs-lookup"><span data-stu-id="62fa1-199">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="62fa1-200">**number**</span><span class="sxs-lookup"><span data-stu-id="62fa1-200">**number**</span></span>        | <span data-ttu-id="62fa1-201">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="62fa1-201">[numberColumn][]</span></span>        | <span data-ttu-id="62fa1-202">Esta coluna armazena valores numéricos.</span><span class="sxs-lookup"><span data-stu-id="62fa1-202">This column stores number values.</span></span>
| <span data-ttu-id="62fa1-203">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="62fa1-203">**personOrGroup**</span></span> | <span data-ttu-id="62fa1-204">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="62fa1-204">[personOrGroupColumn][]</span></span> | <span data-ttu-id="62fa1-205">Esta coluna armazena valores de Pessoa ou Grupo.</span><span class="sxs-lookup"><span data-stu-id="62fa1-205">This column stores Person or Group values.</span></span>
| <span data-ttu-id="62fa1-206">**text**</span><span class="sxs-lookup"><span data-stu-id="62fa1-206">**text**</span></span>          | <span data-ttu-id="62fa1-207">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="62fa1-207">[textColumn][]</span></span>          | <span data-ttu-id="62fa1-208">Esta coluna armazena valores de texto.</span><span class="sxs-lookup"><span data-stu-id="62fa1-208">This column stores text values.</span></span>
| <span data-ttu-id="62fa1-209">**isDeletable**</span><span class="sxs-lookup"><span data-stu-id="62fa1-209">**isDeletable**</span></span>       | <span data-ttu-id="62fa1-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="62fa1-210">Boolean</span></span> | <span data-ttu-id="62fa1-211">Indica se essa coluna pode ser excluída.</span><span class="sxs-lookup"><span data-stu-id="62fa1-211">Indicates whether this column can be deleted.</span></span>
| <span data-ttu-id="62fa1-212">**propagateChanges**</span><span class="sxs-lookup"><span data-stu-id="62fa1-212">**propagateChanges**</span></span>     | <span data-ttu-id="62fa1-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="62fa1-213">Boolean</span></span> | <span data-ttu-id="62fa1-214">Se `true` , as alterações nesta coluna serão propagadas para listas que implementam a coluna.</span><span class="sxs-lookup"><span data-stu-id="62fa1-214">If `true`, changes to this column will be propagated to lists that implement the column.</span></span> 
| <span data-ttu-id="62fa1-215">**isReorderable**</span><span class="sxs-lookup"><span data-stu-id="62fa1-215">**isReorderable**</span></span>         | <span data-ttu-id="62fa1-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="62fa1-216">Boolean</span></span> | <span data-ttu-id="62fa1-217">Indica se os valores na coluna podem ser reordenados.</span><span class="sxs-lookup"><span data-stu-id="62fa1-217">Indicates whether values in the column can be reordered.</span></span> <span data-ttu-id="62fa1-218">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="62fa1-218">Read-only.</span></span>
| <span data-ttu-id="62fa1-219">**isSealed**</span><span class="sxs-lookup"><span data-stu-id="62fa1-219">**isSealed**</span></span>              | <span data-ttu-id="62fa1-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="62fa1-220">Boolean</span></span> | <span data-ttu-id="62fa1-221">Especifica se a coluna pode ser alterada.</span><span class="sxs-lookup"><span data-stu-id="62fa1-221">Specifies whether the column can be changed.</span></span>
| <span data-ttu-id="62fa1-222">**validation**</span><span class="sxs-lookup"><span data-stu-id="62fa1-222">**validation**</span></span>   |  <span data-ttu-id="62fa1-223">[columnValidation][]</span><span class="sxs-lookup"><span data-stu-id="62fa1-223">[columnValidation][]</span></span>    | <span data-ttu-id="62fa1-224">Esta coluna armazena a fórmula e a mensagem de validação da coluna.</span><span class="sxs-lookup"><span data-stu-id="62fa1-224">This column stores validation formula and message for the column.</span></span> 
| <span data-ttu-id="62fa1-225">**hyperlinkOrPicture**</span><span class="sxs-lookup"><span data-stu-id="62fa1-225">**hyperlinkOrPicture**</span></span>  | <span data-ttu-id="62fa1-226">[hyperlinkOrPictureColumn][]</span><span class="sxs-lookup"><span data-stu-id="62fa1-226">[hyperlinkOrPictureColumn][]</span></span> | <span data-ttu-id="62fa1-227">Esta coluna armazena valores de hiperlink ou imagem.</span><span class="sxs-lookup"><span data-stu-id="62fa1-227">This column stores hyperlink or picture values.</span></span> 
| <span data-ttu-id="62fa1-228">**term**</span><span class="sxs-lookup"><span data-stu-id="62fa1-228">**term**</span></span>     | <span data-ttu-id="62fa1-229">[termColumn][]</span><span class="sxs-lookup"><span data-stu-id="62fa1-229">[termColumn][]</span></span> | <span data-ttu-id="62fa1-230">Esta coluna armazena termos de taxonomia.</span><span class="sxs-lookup"><span data-stu-id="62fa1-230">This column stores taxonomy terms.</span></span>
| <span data-ttu-id="62fa1-231">**sourceContentType**</span><span class="sxs-lookup"><span data-stu-id="62fa1-231">**sourceContentType**</span></span>   |<span data-ttu-id="62fa1-232">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="62fa1-232">[contentTypeInfo][]</span></span>  | <span data-ttu-id="62fa1-233">ContentType do qual esta coluna é herdada.</span><span class="sxs-lookup"><span data-stu-id="62fa1-233">ContentType from which this column is inherited from.</span></span> <span data-ttu-id="62fa1-234">Usado apenas para buscar colunas contentTypes.</span><span class="sxs-lookup"><span data-stu-id="62fa1-234">Used only to fetch contentTypes columns.</span></span>
| <span data-ttu-id="62fa1-235">**thumbnail**</span><span class="sxs-lookup"><span data-stu-id="62fa1-235">**thumbnail**</span></span>           |<span data-ttu-id="62fa1-236">[thumbnailColumn][]</span><span class="sxs-lookup"><span data-stu-id="62fa1-236">[thumbnailColumn][]</span></span>      | <span data-ttu-id="62fa1-237">Esta coluna armazena valores de miniatura.</span><span class="sxs-lookup"><span data-stu-id="62fa1-237">This column stores thumbnail values.</span></span>
| <span data-ttu-id="62fa1-238">**type**</span><span class="sxs-lookup"><span data-stu-id="62fa1-238">**type**</span></span>         | <span data-ttu-id="62fa1-239">columnTypes</span><span class="sxs-lookup"><span data-stu-id="62fa1-239">columnTypes</span></span>  | <span data-ttu-id="62fa1-240">Para colunas de site, o tipo de coluna.</span><span class="sxs-lookup"><span data-stu-id="62fa1-240">For site columns, the type of column.</span></span> <span data-ttu-id="62fa1-241">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="62fa1-241">Read-only.</span></span>
| <span data-ttu-id="62fa1-242">**contentApprovalStatus**</span><span class="sxs-lookup"><span data-stu-id="62fa1-242">**contentApprovalStatus**</span></span>| <span data-ttu-id="62fa1-243">[contentApprovalStatusColumn][]</span><span class="sxs-lookup"><span data-stu-id="62fa1-243">[contentApprovalStatusColumn][]</span></span>     | <span data-ttu-id="62fa1-244">Esta coluna armazena o status de aprovação de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="62fa1-244">This column stores content approval status.</span></span>

## <a name="relationships"></a><span data-ttu-id="62fa1-245">Relações</span><span class="sxs-lookup"><span data-stu-id="62fa1-245">Relationships</span></span>

| <span data-ttu-id="62fa1-246">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="62fa1-246">Property name</span></span>   | <span data-ttu-id="62fa1-247">Tipo</span><span class="sxs-lookup"><span data-stu-id="62fa1-247">Type</span></span>                      | <span data-ttu-id="62fa1-248">Descrição</span><span class="sxs-lookup"><span data-stu-id="62fa1-248">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="62fa1-249">**sourceColumn**</span><span class="sxs-lookup"><span data-stu-id="62fa1-249">**sourceColumn**</span></span> | <span data-ttu-id="62fa1-250">[columnDefinition][]</span><span class="sxs-lookup"><span data-stu-id="62fa1-250">[columnDefinition][]</span></span> | <span data-ttu-id="62fa1-251">A coluna de origem para a coluna de tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="62fa1-251">The source column for content type column.</span></span>

><span data-ttu-id="62fa1-252">**Observação:** Essas propriedades correspondem à enumeração SharePoint [SPFieldType.][]</span><span class="sxs-lookup"><span data-stu-id="62fa1-252">**Note:** These properties correspond to the SharePoint [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="62fa1-253">Observe que os tipos de campo mais comuns são representados na tabela anterior.</span><span class="sxs-lookup"><span data-stu-id="62fa1-253">Note that the most common field types are represented in the previous table.</span></span> <span data-ttu-id="62fa1-254">No entanto, essa API beta ainda está faltando algumas.</span><span class="sxs-lookup"><span data-stu-id="62fa1-254">However, this beta API is still missing some.</span></span>
<span data-ttu-id="62fa1-255">nestes casos, nenhuma das facetas do tipo de coluna serão preenchidas, e a coluna só terá as propriedades básicas.</span><span class="sxs-lookup"><span data-stu-id="62fa1-255">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="json-representation"></a><span data-ttu-id="62fa1-256">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="62fa1-256">JSON representation</span></span>

<span data-ttu-id="62fa1-257">Aqui está uma representação JSON de um recurso columnDefinition.</span><span class="sxs-lookup"><span data-stu-id="62fa1-257">Here is a JSON representation of a columnDefinition resource.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="62fa1-258">Comentários</span><span class="sxs-lookup"><span data-stu-id="62fa1-258">Remarks</span></span>

<span data-ttu-id="62fa1-259">Os valores ColumnDefinitions e valores de campo para colunas `hidden` não são mostrados por padrão.</span><span class="sxs-lookup"><span data-stu-id="62fa1-259">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="62fa1-260">Para vê-los ao listar **columnDefinitions**, inclua `hidden` na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="62fa1-260">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="62fa1-261">Para vê-los ao exibir valores **field** em [listItems][listItem], inclua as colunas desejadas por nome na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="62fa1-261">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

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

<span data-ttu-id="62fa1-285">
  [SPFieldType]: /previous-versions/office/sharepoint-server/ms428806(v=office.15)</span><span class="sxs-lookup"><span data-stu-id="62fa1-285">[SPFieldType]: /previous-versions/office/sharepoint-server/ms428806(v=office.15)</span></span>

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
