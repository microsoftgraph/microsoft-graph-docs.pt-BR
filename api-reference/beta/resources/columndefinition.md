---
author: JeremyKelley
description: Veja a seguir uma representação JSON de um recurso columnDefinition.
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 7f60d33f8fbfe76c9dfd0ca02c98df96ca6ab380
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973290"
---
# <a name="columndefinition-resource-type"></a><span data-ttu-id="0ddec-103">tipo de recurso columnDefinition</span><span class="sxs-lookup"><span data-stu-id="0ddec-103">columnDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="0ddec-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0ddec-104">JSON representation</span></span>

<span data-ttu-id="0ddec-105">Veja a seguir uma representação JSON de um recurso columnDefinition.</span><span class="sxs-lookup"><span data-stu-id="0ddec-105">Here is a JSON representation of a columnDefinition resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="0ddec-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0ddec-106">Properties</span></span>

<span data-ttu-id="0ddec-107">As colunas podem conter dados de vários tipos.</span><span class="sxs-lookup"><span data-stu-id="0ddec-107">Columns can hold data of various types.</span></span>
<span data-ttu-id="0ddec-108">As propriedades a seguir indicam qual tipo de dados uma coluna armazena, bem como configurações adicionais para esses dados.</span><span class="sxs-lookup"><span data-stu-id="0ddec-108">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="0ddec-109">As propriedades relacionadas ao tipo (Boolean, calculado, Choice, Currency, dateTime, Lookup, Number, personOrGroup, Text) são mutuamente excludentes--uma coluna só pode ter uma delas especificada.</span><span class="sxs-lookup"><span data-stu-id="0ddec-109">The type-related properties (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="0ddec-110">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="0ddec-110">Property name</span></span>           | <span data-ttu-id="0ddec-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ddec-111">Type</span></span>    | <span data-ttu-id="0ddec-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ddec-112">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="0ddec-113">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="0ddec-113">**columnGroup**</span></span>         | <span data-ttu-id="0ddec-114">string</span><span class="sxs-lookup"><span data-stu-id="0ddec-114">string</span></span>  | <span data-ttu-id="0ddec-115">Para colunas de site, o nome do grupo ao qual esta coluna pertence.</span><span class="sxs-lookup"><span data-stu-id="0ddec-115">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="0ddec-116">Ajuda a organizar as colunas relacionadas.</span><span class="sxs-lookup"><span data-stu-id="0ddec-116">Helps organize related columns.</span></span>
| <span data-ttu-id="0ddec-117">**description**</span><span class="sxs-lookup"><span data-stu-id="0ddec-117">**description**</span></span>         | <span data-ttu-id="0ddec-118">string</span><span class="sxs-lookup"><span data-stu-id="0ddec-118">string</span></span>  | <span data-ttu-id="0ddec-119">A descrição voltado para o usuário da coluna.</span><span class="sxs-lookup"><span data-stu-id="0ddec-119">The user-facing description of the column.</span></span>
| <span data-ttu-id="0ddec-120">**displayName**</span><span class="sxs-lookup"><span data-stu-id="0ddec-120">**displayName**</span></span>         | <span data-ttu-id="0ddec-121">string</span><span class="sxs-lookup"><span data-stu-id="0ddec-121">string</span></span>  | <span data-ttu-id="0ddec-122">O nome voltado para o usuário da coluna.</span><span class="sxs-lookup"><span data-stu-id="0ddec-122">The user-facing name of the column.</span></span>
| <span data-ttu-id="0ddec-123">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="0ddec-123">**enforceUniqueValues**</span></span> | <span data-ttu-id="0ddec-124">booliano</span><span class="sxs-lookup"><span data-stu-id="0ddec-124">boolean</span></span> | <span data-ttu-id="0ddec-125">Se for verdadeiro, esse mesmo valor não constará em dois itens de lista nessa coluna.</span><span class="sxs-lookup"><span data-stu-id="0ddec-125">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="0ddec-126">**hidden**</span><span class="sxs-lookup"><span data-stu-id="0ddec-126">**hidden**</span></span>              | <span data-ttu-id="0ddec-127">booliano</span><span class="sxs-lookup"><span data-stu-id="0ddec-127">boolean</span></span> | <span data-ttu-id="0ddec-128">Especifica se a coluna é exibida na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="0ddec-128">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="0ddec-129">**id**</span><span class="sxs-lookup"><span data-stu-id="0ddec-129">**id**</span></span>                  | <span data-ttu-id="0ddec-130">string</span><span class="sxs-lookup"><span data-stu-id="0ddec-130">string</span></span>  | <span data-ttu-id="0ddec-131">O identificador exclusivo da coluna.</span><span class="sxs-lookup"><span data-stu-id="0ddec-131">The unique identifier for the column.</span></span>
| <span data-ttu-id="0ddec-132">**indexed**</span><span class="sxs-lookup"><span data-stu-id="0ddec-132">**indexed**</span></span>             | <span data-ttu-id="0ddec-133">booliano</span><span class="sxs-lookup"><span data-stu-id="0ddec-133">boolean</span></span> | <span data-ttu-id="0ddec-134">Especifica se os valores da coluna podem ser usados para classificação e pesquisa.</span><span class="sxs-lookup"><span data-stu-id="0ddec-134">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="0ddec-135">**name**</span><span class="sxs-lookup"><span data-stu-id="0ddec-135">**name**</span></span>                | <span data-ttu-id="0ddec-136">string</span><span class="sxs-lookup"><span data-stu-id="0ddec-136">string</span></span>  | <span data-ttu-id="0ddec-137">O nome voltado para a API da coluna, conforme ele aparece nos [campos][] em uma [listItem][].</span><span class="sxs-lookup"><span data-stu-id="0ddec-137">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="0ddec-138">Para o nome voltado ao usuário, consulte **displayName**.</span><span class="sxs-lookup"><span data-stu-id="0ddec-138">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="0ddec-139">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="0ddec-139">**readOnly**</span></span>            | <span data-ttu-id="0ddec-140">bool</span><span class="sxs-lookup"><span data-stu-id="0ddec-140">bool</span></span>    | <span data-ttu-id="0ddec-141">Especifica se os valores da coluna podem ser modificados.</span><span class="sxs-lookup"><span data-stu-id="0ddec-141">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="0ddec-142">**required**</span><span class="sxs-lookup"><span data-stu-id="0ddec-142">**required**</span></span>            | <span data-ttu-id="0ddec-143">booliano</span><span class="sxs-lookup"><span data-stu-id="0ddec-143">boolean</span></span> | <span data-ttu-id="0ddec-144">Especifica se o valor da coluna não é opcional.</span><span class="sxs-lookup"><span data-stu-id="0ddec-144">Specifies whether the column value is not optional.</span></span>
| <span data-ttu-id="0ddec-145">**boolean**</span><span class="sxs-lookup"><span data-stu-id="0ddec-145">**boolean**</span></span>       | <span data-ttu-id="0ddec-146">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="0ddec-146">[booleanColumn][]</span></span>       | <span data-ttu-id="0ddec-147">Esta coluna armazena valores boolianos.</span><span class="sxs-lookup"><span data-stu-id="0ddec-147">This column stores boolean values.</span></span>
| <span data-ttu-id="0ddec-148">**calculated**</span><span class="sxs-lookup"><span data-stu-id="0ddec-148">**calculated**</span></span>    | <span data-ttu-id="0ddec-149">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="0ddec-149">[calculatedColumn][]</span></span>    | <span data-ttu-id="0ddec-150">Os dados dessa coluna são calculados com base em outras colunas.</span><span class="sxs-lookup"><span data-stu-id="0ddec-150">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="0ddec-151">**choice**</span><span class="sxs-lookup"><span data-stu-id="0ddec-151">**choice**</span></span>        | <span data-ttu-id="0ddec-152">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="0ddec-152">[choiceColumn][]</span></span>        | <span data-ttu-id="0ddec-153">Esta coluna armazena dados de uma lista de opções.</span><span class="sxs-lookup"><span data-stu-id="0ddec-153">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="0ddec-154">**currency**</span><span class="sxs-lookup"><span data-stu-id="0ddec-154">**currency**</span></span>      | <span data-ttu-id="0ddec-155">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="0ddec-155">[currencyColumn][]</span></span>      | <span data-ttu-id="0ddec-156">Esta coluna armazena valores monetários.</span><span class="sxs-lookup"><span data-stu-id="0ddec-156">This column stores currency values.</span></span>
| <span data-ttu-id="0ddec-157">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="0ddec-157">**dateTime**</span></span>      | <span data-ttu-id="0ddec-158">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="0ddec-158">[dateTimeColumn][]</span></span>      | <span data-ttu-id="0ddec-159">Esta coluna armazena valores de datetime.</span><span class="sxs-lookup"><span data-stu-id="0ddec-159">This column stores DateTime values.</span></span>
| <span data-ttu-id="0ddec-160">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="0ddec-160">**defaultValue**</span></span>  | <span data-ttu-id="0ddec-161">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="0ddec-161">[defaultColumnValue][]</span></span>  | <span data-ttu-id="0ddec-162">O valor padrão dessa coluna.</span><span class="sxs-lookup"><span data-stu-id="0ddec-162">The default value for this column.</span></span>
| <span data-ttu-id="0ddec-163">**localização geográfica**</span><span class="sxs-lookup"><span data-stu-id="0ddec-163">**geolocation**</span></span>   | <span data-ttu-id="0ddec-164">[geolocationColumn][]</span><span class="sxs-lookup"><span data-stu-id="0ddec-164">[geolocationColumn][]</span></span>   | <span data-ttu-id="0ddec-165">Esta coluna armazena uma localização geográfica.</span><span class="sxs-lookup"><span data-stu-id="0ddec-165">This column stores a geolocation.</span></span>
| <span data-ttu-id="0ddec-166">**lookup**</span><span class="sxs-lookup"><span data-stu-id="0ddec-166">**lookup**</span></span>        | <span data-ttu-id="0ddec-167">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="0ddec-167">[lookupColumn][]</span></span>        | <span data-ttu-id="0ddec-168">Os dados dessa coluna são procurados por outra fonte no site.</span><span class="sxs-lookup"><span data-stu-id="0ddec-168">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="0ddec-169">**number**</span><span class="sxs-lookup"><span data-stu-id="0ddec-169">**number**</span></span>        | <span data-ttu-id="0ddec-170">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="0ddec-170">[numberColumn][]</span></span>        | <span data-ttu-id="0ddec-171">Esta coluna armazena valores numéricos.</span><span class="sxs-lookup"><span data-stu-id="0ddec-171">This column stores number values.</span></span>
| <span data-ttu-id="0ddec-172">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="0ddec-172">**personOrGroup**</span></span> | <span data-ttu-id="0ddec-173">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="0ddec-173">[personOrGroupColumn][]</span></span> | <span data-ttu-id="0ddec-174">Esta coluna armazena valores de Pessoa ou Grupo.</span><span class="sxs-lookup"><span data-stu-id="0ddec-174">This column stores Person or Group values.</span></span>
| <span data-ttu-id="0ddec-175">**text**</span><span class="sxs-lookup"><span data-stu-id="0ddec-175">**text**</span></span>          | <span data-ttu-id="0ddec-176">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="0ddec-176">[textColumn][]</span></span>          | <span data-ttu-id="0ddec-177">Esta coluna armazena valores de texto.</span><span class="sxs-lookup"><span data-stu-id="0ddec-177">This column stores text values.</span></span>

><span data-ttu-id="0ddec-178">**Observação:** Essas propriedades correspondem à enumeração de [][] UserField do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0ddec-178">**Note:** These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="0ddec-179">Enquanto os tipos de campo mais comuns são representados na tabela anterior, esta API beta ainda não tem alguns.</span><span class="sxs-lookup"><span data-stu-id="0ddec-179">While the most common field types are represented in the previous table, this beta API is still missing some.</span></span>
<span data-ttu-id="0ddec-180">nestes casos, nenhuma das facetas do tipo de coluna serão preenchidas, e a coluna só terá as propriedades básicas.</span><span class="sxs-lookup"><span data-stu-id="0ddec-180">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="0ddec-181">Comentários</span><span class="sxs-lookup"><span data-stu-id="0ddec-181">Remarks</span></span>

<span data-ttu-id="0ddec-182">Os valores ColumnDefinitions e valores de campo para colunas `hidden` não são mostrados por padrão.</span><span class="sxs-lookup"><span data-stu-id="0ddec-182">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="0ddec-183">Para vê-los ao listar **columnDefinitions**, inclua `hidden` na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="0ddec-183">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="0ddec-184">Para vê-los ao exibir valores **field** em [listItems][listItem], inclua as colunas desejadas por nome na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="0ddec-184">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

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

<span data-ttu-id="0ddec-198">
  [SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx</span><span class="sxs-lookup"><span data-stu-id="0ddec-198">[SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx</span></span>

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
