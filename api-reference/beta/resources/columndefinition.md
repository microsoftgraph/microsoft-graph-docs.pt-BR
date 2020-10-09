---
author: JeremyKelley
description: Veja a seguir uma representação JSON de um recurso columnDefinition.
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: d6034bfc85c7c2c1e93d0557fdf508fd1ea1ff46
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401684"
---
# <a name="columndefinition-resource-type"></a><span data-ttu-id="e028c-103">tipo de recurso columnDefinition</span><span class="sxs-lookup"><span data-stu-id="e028c-103">columnDefinition resource type</span></span>

<span data-ttu-id="e028c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e028c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="e028c-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e028c-105">JSON representation</span></span>

<span data-ttu-id="e028c-106">Veja a seguir uma representação JSON de um recurso columnDefinition.</span><span class="sxs-lookup"><span data-stu-id="e028c-106">Here is a JSON representation of a columnDefinition resource.</span></span>

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
  "enforceUniqueValues": "true",
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
  "text": { "@odata.type": "microsoft.graph.textColumn" }
}
```

## <a name="properties"></a><span data-ttu-id="e028c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e028c-107">Properties</span></span>

<span data-ttu-id="e028c-108">As colunas podem conter dados de vários tipos.</span><span class="sxs-lookup"><span data-stu-id="e028c-108">Columns can hold data of various types.</span></span>
<span data-ttu-id="e028c-109">As propriedades a seguir indicam qual tipo de dados uma coluna armazena, bem como configurações adicionais para esses dados.</span><span class="sxs-lookup"><span data-stu-id="e028c-109">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="e028c-110">As propriedades relacionadas ao tipo (Boolean, calculado, Choice, Currency, dateTime, Lookup, Number, personOrGroup, Text) são mutuamente excludentes--uma coluna só pode ter uma delas especificada.</span><span class="sxs-lookup"><span data-stu-id="e028c-110">The type-related properties (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="e028c-111">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="e028c-111">Property name</span></span>           | <span data-ttu-id="e028c-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="e028c-112">Type</span></span>    | <span data-ttu-id="e028c-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="e028c-113">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="e028c-114">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="e028c-114">**columnGroup**</span></span>         | <span data-ttu-id="e028c-115">string</span><span class="sxs-lookup"><span data-stu-id="e028c-115">string</span></span>  | <span data-ttu-id="e028c-116">Para colunas de site, o nome do grupo ao qual esta coluna pertence.</span><span class="sxs-lookup"><span data-stu-id="e028c-116">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="e028c-117">Ajuda a organizar as colunas relacionadas.</span><span class="sxs-lookup"><span data-stu-id="e028c-117">Helps organize related columns.</span></span>
| <span data-ttu-id="e028c-118">**description**</span><span class="sxs-lookup"><span data-stu-id="e028c-118">**description**</span></span>         | <span data-ttu-id="e028c-119">string</span><span class="sxs-lookup"><span data-stu-id="e028c-119">string</span></span>  | <span data-ttu-id="e028c-120">A descrição voltado para o usuário da coluna.</span><span class="sxs-lookup"><span data-stu-id="e028c-120">The user-facing description of the column.</span></span>
| <span data-ttu-id="e028c-121">**displayName**</span><span class="sxs-lookup"><span data-stu-id="e028c-121">**displayName**</span></span>         | <span data-ttu-id="e028c-122">string</span><span class="sxs-lookup"><span data-stu-id="e028c-122">string</span></span>  | <span data-ttu-id="e028c-123">O nome voltado para o usuário da coluna.</span><span class="sxs-lookup"><span data-stu-id="e028c-123">The user-facing name of the column.</span></span>
| <span data-ttu-id="e028c-124">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="e028c-124">**enforceUniqueValues**</span></span> | <span data-ttu-id="e028c-125">booliano</span><span class="sxs-lookup"><span data-stu-id="e028c-125">boolean</span></span> | <span data-ttu-id="e028c-126">Se for verdadeiro, esse mesmo valor não constará em dois itens de lista nessa coluna.</span><span class="sxs-lookup"><span data-stu-id="e028c-126">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="e028c-127">**hidden**</span><span class="sxs-lookup"><span data-stu-id="e028c-127">**hidden**</span></span>              | <span data-ttu-id="e028c-128">booliano</span><span class="sxs-lookup"><span data-stu-id="e028c-128">boolean</span></span> | <span data-ttu-id="e028c-129">Especifica se a coluna é exibida na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="e028c-129">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="e028c-130">**id**</span><span class="sxs-lookup"><span data-stu-id="e028c-130">**id**</span></span>                  | <span data-ttu-id="e028c-131">string</span><span class="sxs-lookup"><span data-stu-id="e028c-131">string</span></span>  | <span data-ttu-id="e028c-132">O identificador exclusivo da coluna.</span><span class="sxs-lookup"><span data-stu-id="e028c-132">The unique identifier for the column.</span></span>
| <span data-ttu-id="e028c-133">**indexed**</span><span class="sxs-lookup"><span data-stu-id="e028c-133">**indexed**</span></span>             | <span data-ttu-id="e028c-134">booliano</span><span class="sxs-lookup"><span data-stu-id="e028c-134">boolean</span></span> | <span data-ttu-id="e028c-135">Especifica se os valores da coluna podem ser usados para classificação e pesquisa.</span><span class="sxs-lookup"><span data-stu-id="e028c-135">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="e028c-136">**name**</span><span class="sxs-lookup"><span data-stu-id="e028c-136">**name**</span></span>                | <span data-ttu-id="e028c-137">string</span><span class="sxs-lookup"><span data-stu-id="e028c-137">string</span></span>  | <span data-ttu-id="e028c-138">O nome voltado para a API da coluna, conforme ele aparece nos [campos][] em uma [listItem][].</span><span class="sxs-lookup"><span data-stu-id="e028c-138">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="e028c-139">Para o nome voltado ao usuário, consulte **displayName**.</span><span class="sxs-lookup"><span data-stu-id="e028c-139">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="e028c-140">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="e028c-140">**readOnly**</span></span>            | <span data-ttu-id="e028c-141">bool</span><span class="sxs-lookup"><span data-stu-id="e028c-141">bool</span></span>    | <span data-ttu-id="e028c-142">Especifica se os valores da coluna podem ser modificados.</span><span class="sxs-lookup"><span data-stu-id="e028c-142">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="e028c-143">**required**</span><span class="sxs-lookup"><span data-stu-id="e028c-143">**required**</span></span>            | <span data-ttu-id="e028c-144">booliano</span><span class="sxs-lookup"><span data-stu-id="e028c-144">boolean</span></span> | <span data-ttu-id="e028c-145">Especifica se o valor da coluna não é opcional.</span><span class="sxs-lookup"><span data-stu-id="e028c-145">Specifies whether the column value is not optional.</span></span>
| <span data-ttu-id="e028c-146">**boolean**</span><span class="sxs-lookup"><span data-stu-id="e028c-146">**boolean**</span></span>       | <span data-ttu-id="e028c-147">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="e028c-147">[booleanColumn][]</span></span>       | <span data-ttu-id="e028c-148">Esta coluna armazena valores boolianos.</span><span class="sxs-lookup"><span data-stu-id="e028c-148">This column stores boolean values.</span></span>
| <span data-ttu-id="e028c-149">**calculated**</span><span class="sxs-lookup"><span data-stu-id="e028c-149">**calculated**</span></span>    | <span data-ttu-id="e028c-150">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="e028c-150">[calculatedColumn][]</span></span>    | <span data-ttu-id="e028c-151">Os dados dessa coluna são calculados com base em outras colunas.</span><span class="sxs-lookup"><span data-stu-id="e028c-151">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="e028c-152">**choice**</span><span class="sxs-lookup"><span data-stu-id="e028c-152">**choice**</span></span>        | <span data-ttu-id="e028c-153">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="e028c-153">[choiceColumn][]</span></span>        | <span data-ttu-id="e028c-154">Esta coluna armazena dados de uma lista de opções.</span><span class="sxs-lookup"><span data-stu-id="e028c-154">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="e028c-155">**currency**</span><span class="sxs-lookup"><span data-stu-id="e028c-155">**currency**</span></span>      | <span data-ttu-id="e028c-156">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="e028c-156">[currencyColumn][]</span></span>      | <span data-ttu-id="e028c-157">Esta coluna armazena valores monetários.</span><span class="sxs-lookup"><span data-stu-id="e028c-157">This column stores currency values.</span></span>
| <span data-ttu-id="e028c-158">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="e028c-158">**dateTime**</span></span>      | <span data-ttu-id="e028c-159">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="e028c-159">[dateTimeColumn][]</span></span>      | <span data-ttu-id="e028c-160">Esta coluna armazena valores de datetime.</span><span class="sxs-lookup"><span data-stu-id="e028c-160">This column stores DateTime values.</span></span>
| <span data-ttu-id="e028c-161">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="e028c-161">**defaultValue**</span></span>  | <span data-ttu-id="e028c-162">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="e028c-162">[defaultColumnValue][]</span></span>  | <span data-ttu-id="e028c-163">O valor padrão dessa coluna.</span><span class="sxs-lookup"><span data-stu-id="e028c-163">The default value for this column.</span></span>
| <span data-ttu-id="e028c-164">**localização geográfica**</span><span class="sxs-lookup"><span data-stu-id="e028c-164">**geolocation**</span></span>   | <span data-ttu-id="e028c-165">[geolocationColumn][]</span><span class="sxs-lookup"><span data-stu-id="e028c-165">[geolocationColumn][]</span></span>   | <span data-ttu-id="e028c-166">Esta coluna armazena uma localização geográfica.</span><span class="sxs-lookup"><span data-stu-id="e028c-166">This column stores a geolocation.</span></span>
| <span data-ttu-id="e028c-167">**lookup**</span><span class="sxs-lookup"><span data-stu-id="e028c-167">**lookup**</span></span>        | <span data-ttu-id="e028c-168">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="e028c-168">[lookupColumn][]</span></span>        | <span data-ttu-id="e028c-169">Os dados dessa coluna são procurados por outra fonte no site.</span><span class="sxs-lookup"><span data-stu-id="e028c-169">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="e028c-170">**number**</span><span class="sxs-lookup"><span data-stu-id="e028c-170">**number**</span></span>        | <span data-ttu-id="e028c-171">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="e028c-171">[numberColumn][]</span></span>        | <span data-ttu-id="e028c-172">Esta coluna armazena valores numéricos.</span><span class="sxs-lookup"><span data-stu-id="e028c-172">This column stores number values.</span></span>
| <span data-ttu-id="e028c-173">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="e028c-173">**personOrGroup**</span></span> | <span data-ttu-id="e028c-174">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="e028c-174">[personOrGroupColumn][]</span></span> | <span data-ttu-id="e028c-175">Esta coluna armazena valores de Pessoa ou Grupo.</span><span class="sxs-lookup"><span data-stu-id="e028c-175">This column stores Person or Group values.</span></span>
| <span data-ttu-id="e028c-176">**text**</span><span class="sxs-lookup"><span data-stu-id="e028c-176">**text**</span></span>          | <span data-ttu-id="e028c-177">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="e028c-177">[textColumn][]</span></span>          | <span data-ttu-id="e028c-178">Esta coluna armazena valores de texto.</span><span class="sxs-lookup"><span data-stu-id="e028c-178">This column stores text values.</span></span>

><span data-ttu-id="e028c-179">**Observação:** Essas propriedades correspondem à enumeração de [UserField][] do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e028c-179">**Note:** These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="e028c-180">Enquanto os tipos de campo mais comuns são representados na tabela anterior, esta API beta ainda não tem alguns.</span><span class="sxs-lookup"><span data-stu-id="e028c-180">While the most common field types are represented in the previous table, this beta API is still missing some.</span></span>
<span data-ttu-id="e028c-181">nestes casos, nenhuma das facetas do tipo de coluna serão preenchidas, e a coluna só terá as propriedades básicas.</span><span class="sxs-lookup"><span data-stu-id="e028c-181">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="e028c-182">Comentários</span><span class="sxs-lookup"><span data-stu-id="e028c-182">Remarks</span></span>

<span data-ttu-id="e028c-183">Os valores ColumnDefinitions e valores de campo para colunas `hidden` não são mostrados por padrão.</span><span class="sxs-lookup"><span data-stu-id="e028c-183">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="e028c-184">Para vê-los ao listar **columnDefinitions**, inclua `hidden` na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="e028c-184">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="e028c-185">Para vê-los ao exibir valores **field** em [listItems][listItem], inclua as colunas desejadas por nome na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="e028c-185">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

[booleanColumn]: booleancolumn.md
[calculatedColumn]: calculatedcolumn.md
[choiceColumn]: choicecolumn.md
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

<span data-ttu-id="e028c-199">
  [SPFieldType]: /previous-versions/office/sharepoint-server/ms428806(v=office.15)</span><span class="sxs-lookup"><span data-stu-id="e028c-199">[SPFieldType]: /previous-versions/office/sharepoint-server/ms428806(v=office.15)</span></span>

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