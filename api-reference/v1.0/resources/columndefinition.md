---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
description: Aqui está uma representação JSON de um recurso ColumnDefinition.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3a02721c5289b1d49077e1b2d9fa1017f0c53021
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032869"
---
# <a name="columndefinition-resource"></a><span data-ttu-id="1736f-103">Recurso ColumnDefinition</span><span class="sxs-lookup"><span data-stu-id="1736f-103">ColumnDefinition resource</span></span>

## <a name="json-representation"></a><span data-ttu-id="1736f-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1736f-104">JSON representation</span></span>

<span data-ttu-id="1736f-105">Aqui está uma representação JSON de um recurso ColumnDefinition.</span><span class="sxs-lookup"><span data-stu-id="1736f-105">Here is a JSON representation of a ColumnDefinition resource.</span></span>

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
  "lookup": { "@odata.type": "microsoft.graph.lookupColumn" },
  "number": { "@odata.type": "microsoft.graph.numberColumn" },
  "personOrGroup": { "@odata.type": "microsoft.graph.personOrGroupColumn" },
  "text": { "@odata.type": "microsoft.graph.textColumn" }
}
```

## <a name="properties"></a><span data-ttu-id="1736f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1736f-106">Properties</span></span>

<span data-ttu-id="1736f-107">O recurso **columnDefinition** tem as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="1736f-107">The **columnDefinition** resource has the following properties.</span></span>

| <span data-ttu-id="1736f-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="1736f-108">Property name</span></span>           | <span data-ttu-id="1736f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1736f-109">Type</span></span>    | <span data-ttu-id="1736f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1736f-110">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="1736f-111">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="1736f-111">**columnGroup**</span></span>         | <span data-ttu-id="1736f-112">string</span><span class="sxs-lookup"><span data-stu-id="1736f-112">string</span></span>  | <span data-ttu-id="1736f-113">Para colunas de site, o nome do grupo ao qual esta coluna pertence.</span><span class="sxs-lookup"><span data-stu-id="1736f-113">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="1736f-114">Ajuda a organizar as colunas relacionadas.</span><span class="sxs-lookup"><span data-stu-id="1736f-114">Helps organize related columns.</span></span>
| <span data-ttu-id="1736f-115">**description**</span><span class="sxs-lookup"><span data-stu-id="1736f-115">**description**</span></span>         | <span data-ttu-id="1736f-116">string</span><span class="sxs-lookup"><span data-stu-id="1736f-116">string</span></span>  | <span data-ttu-id="1736f-117">A descrição voltado para o usuário da coluna.</span><span class="sxs-lookup"><span data-stu-id="1736f-117">The user-facing description of the column.</span></span>
| <span data-ttu-id="1736f-118">**displayName**</span><span class="sxs-lookup"><span data-stu-id="1736f-118">**displayName**</span></span>         | <span data-ttu-id="1736f-119">string</span><span class="sxs-lookup"><span data-stu-id="1736f-119">string</span></span>  | <span data-ttu-id="1736f-120">O nome voltado para o usuário da coluna.</span><span class="sxs-lookup"><span data-stu-id="1736f-120">The user-facing name of the column.</span></span>
| <span data-ttu-id="1736f-121">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="1736f-121">**enforceUniqueValues**</span></span> | <span data-ttu-id="1736f-122">booliano</span><span class="sxs-lookup"><span data-stu-id="1736f-122">boolean</span></span> | <span data-ttu-id="1736f-123">Se for verdadeiro, esse mesmo valor não constará em dois itens de lista nessa coluna.</span><span class="sxs-lookup"><span data-stu-id="1736f-123">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="1736f-124">**hidden**</span><span class="sxs-lookup"><span data-stu-id="1736f-124">**hidden**</span></span>              | <span data-ttu-id="1736f-125">booliano</span><span class="sxs-lookup"><span data-stu-id="1736f-125">boolean</span></span> | <span data-ttu-id="1736f-126">Especifica se a coluna é exibida na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="1736f-126">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="1736f-127">**id**</span><span class="sxs-lookup"><span data-stu-id="1736f-127">**id**</span></span>                  | <span data-ttu-id="1736f-128">string</span><span class="sxs-lookup"><span data-stu-id="1736f-128">string</span></span>  | <span data-ttu-id="1736f-129">O identificador exclusivo da coluna.</span><span class="sxs-lookup"><span data-stu-id="1736f-129">The unique identifier for the column.</span></span>
| <span data-ttu-id="1736f-130">**indexed**</span><span class="sxs-lookup"><span data-stu-id="1736f-130">**indexed**</span></span>             | <span data-ttu-id="1736f-131">booliano</span><span class="sxs-lookup"><span data-stu-id="1736f-131">boolean</span></span> | <span data-ttu-id="1736f-132">Especifica se os valores da coluna podem ser usados para classificação e pesquisa.</span><span class="sxs-lookup"><span data-stu-id="1736f-132">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="1736f-133">**name**</span><span class="sxs-lookup"><span data-stu-id="1736f-133">**name**</span></span>                | <span data-ttu-id="1736f-134">string</span><span class="sxs-lookup"><span data-stu-id="1736f-134">string</span></span>  | <span data-ttu-id="1736f-135">O nome voltado para a API da coluna, conforme ele aparece nos [campos][] em uma [listItem][].</span><span class="sxs-lookup"><span data-stu-id="1736f-135">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="1736f-136">Para o nome voltado ao usuário, consulte **displayName**.</span><span class="sxs-lookup"><span data-stu-id="1736f-136">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="1736f-137">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="1736f-137">**readOnly**</span></span>            | <span data-ttu-id="1736f-138">bool</span><span class="sxs-lookup"><span data-stu-id="1736f-138">bool</span></span>    | <span data-ttu-id="1736f-139">Especifica se os valores da coluna podem ser modificados.</span><span class="sxs-lookup"><span data-stu-id="1736f-139">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="1736f-140">**required**</span><span class="sxs-lookup"><span data-stu-id="1736f-140">**required**</span></span>            | <span data-ttu-id="1736f-141">booliano</span><span class="sxs-lookup"><span data-stu-id="1736f-141">boolean</span></span> | <span data-ttu-id="1736f-142">Especifica se o valor da coluna não é opcional.</span><span class="sxs-lookup"><span data-stu-id="1736f-142">Specifies whether the column value is not optional.</span></span>

<span data-ttu-id="1736f-143">As colunas podem conter dados de vários tipos.</span><span class="sxs-lookup"><span data-stu-id="1736f-143">Columns can hold data of various types.</span></span>
<span data-ttu-id="1736f-144">As propriedades a seguir indicam qual tipo de dados uma coluna armazena, bem como configurações adicionais para esses dados.</span><span class="sxs-lookup"><span data-stu-id="1736f-144">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="1736f-145">Essas propriedades são mutuamente exclusivas: uma coluna só pode ter uma delas especificada.</span><span class="sxs-lookup"><span data-stu-id="1736f-145">These properties are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="1736f-146">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="1736f-146">Property name</span></span>     | <span data-ttu-id="1736f-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="1736f-147">Type</span></span>                    | <span data-ttu-id="1736f-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="1736f-148">Description</span></span>
|:------------------|:------------------------|:-------------------------------
| <span data-ttu-id="1736f-149">**boolean**</span><span class="sxs-lookup"><span data-stu-id="1736f-149">**boolean**</span></span>       | <span data-ttu-id="1736f-150">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="1736f-150">[booleanColumn][]</span></span>       | <span data-ttu-id="1736f-151">Esta coluna armazena valores boolianos.</span><span class="sxs-lookup"><span data-stu-id="1736f-151">This column stores boolean values.</span></span>
| <span data-ttu-id="1736f-152">**calculated**</span><span class="sxs-lookup"><span data-stu-id="1736f-152">**calculated**</span></span>    | <span data-ttu-id="1736f-153">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="1736f-153">[calculatedColumn][]</span></span>    | <span data-ttu-id="1736f-154">Os dados dessa coluna são calculados com base em outras colunas.</span><span class="sxs-lookup"><span data-stu-id="1736f-154">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="1736f-155">**choice**</span><span class="sxs-lookup"><span data-stu-id="1736f-155">**choice**</span></span>        | <span data-ttu-id="1736f-156">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="1736f-156">[choiceColumn][]</span></span>        | <span data-ttu-id="1736f-157">Esta coluna armazena dados de uma lista de opções.</span><span class="sxs-lookup"><span data-stu-id="1736f-157">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="1736f-158">**currency**</span><span class="sxs-lookup"><span data-stu-id="1736f-158">**currency**</span></span>      | <span data-ttu-id="1736f-159">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="1736f-159">[currencyColumn][]</span></span>      | <span data-ttu-id="1736f-160">Esta coluna armazena valores monetários.</span><span class="sxs-lookup"><span data-stu-id="1736f-160">This column stores currency values.</span></span>
| <span data-ttu-id="1736f-161">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="1736f-161">**dateTime**</span></span>      | <span data-ttu-id="1736f-162">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="1736f-162">[dateTimeColumn][]</span></span>      | <span data-ttu-id="1736f-163">Esta coluna armazena valores de datetime.</span><span class="sxs-lookup"><span data-stu-id="1736f-163">This column stores DateTime values.</span></span>
| <span data-ttu-id="1736f-164">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="1736f-164">**defaultValue**</span></span>  | <span data-ttu-id="1736f-165">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="1736f-165">[defaultColumnValue][]</span></span>  | <span data-ttu-id="1736f-166">O valor padrão dessa coluna.</span><span class="sxs-lookup"><span data-stu-id="1736f-166">The default value for this column.</span></span>
| <span data-ttu-id="1736f-167">**lookup**</span><span class="sxs-lookup"><span data-stu-id="1736f-167">**lookup**</span></span>        | <span data-ttu-id="1736f-168">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="1736f-168">[lookupColumn][]</span></span>        | <span data-ttu-id="1736f-169">Os dados dessa coluna são procurados por outra fonte no site.</span><span class="sxs-lookup"><span data-stu-id="1736f-169">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="1736f-170">**number**</span><span class="sxs-lookup"><span data-stu-id="1736f-170">**number**</span></span>        | <span data-ttu-id="1736f-171">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="1736f-171">[numberColumn][]</span></span>        | <span data-ttu-id="1736f-172">Esta coluna armazena valores numéricos.</span><span class="sxs-lookup"><span data-stu-id="1736f-172">This column stores number values.</span></span>
| <span data-ttu-id="1736f-173">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="1736f-173">**personOrGroup**</span></span> | <span data-ttu-id="1736f-174">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="1736f-174">[personOrGroupColumn][]</span></span> | <span data-ttu-id="1736f-175">Esta coluna armazena valores de Pessoa ou Grupo.</span><span class="sxs-lookup"><span data-stu-id="1736f-175">This column stores Person or Group values.</span></span>
| <span data-ttu-id="1736f-176">**text**</span><span class="sxs-lookup"><span data-stu-id="1736f-176">**text**</span></span>          | <span data-ttu-id="1736f-177">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="1736f-177">[textColumn][]</span></span>          | <span data-ttu-id="1736f-178">Esta coluna armazena valores de texto.</span><span class="sxs-lookup"><span data-stu-id="1736f-178">This column stores text values.</span></span>

<span data-ttu-id="1736f-179">Observação: essas propriedades correspondem à enumeração [SPFieldType][] do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1736f-179">Note: These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="1736f-180">Embora os tipos de campo mais comuns sejam representados acima, essa API ainda não tem alguns.</span><span class="sxs-lookup"><span data-stu-id="1736f-180">While the most common field types are represented above, this API is still missing some.</span></span>
<span data-ttu-id="1736f-181">nestes casos, nenhuma das facetas do tipo de coluna serão preenchidas, e a coluna só terá as propriedades básicas.</span><span class="sxs-lookup"><span data-stu-id="1736f-181">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="1736f-182">Comentários</span><span class="sxs-lookup"><span data-stu-id="1736f-182">Remarks</span></span>

<span data-ttu-id="1736f-183">Os valores ColumnDefinitions e valores de campo para colunas `hidden` não são mostrados por padrão.</span><span class="sxs-lookup"><span data-stu-id="1736f-183">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="1736f-184">Para vê-los ao listar **columnDefinitions**, inclua `hidden` na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="1736f-184">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="1736f-185">Para vê-los ao exibir valores **field** em [listItems][listItem], inclua as colunas desejadas por nome na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="1736f-185">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

[booleanColumn]: booleancolumn.md
[calculatedColumn]: calculatedcolumn.md
[choiceColumn]: choicecolumn.md
[currencyColumn]: currencycolumn.md
[dateTimeColumn]: datetimecolumn.md
[defaultColumnValue]: defaultcolumnvalue.md
[lookupColumn]: lookupcolumn.md
[numberColumn]: numbercolumn.md
[personOrGroupColumn]: personorgroupcolumn.md
[textColumn]: textcolumn.md
[fieldValueSet]: fieldvalueset.md
[campos]: fieldvalueset.md
[fields]: fieldvalueset.md
[listItem]: listitem.md

<span data-ttu-id="1736f-198">
  [SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx</span><span class="sxs-lookup"><span data-stu-id="1736f-198">[SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition"
} -->
