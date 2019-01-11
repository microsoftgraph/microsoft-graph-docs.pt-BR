---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
ms.openlocfilehash: 598a781c25dd9271be84eb3dfc16b1e5ff439298
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862878"
---
# <a name="columndefinition-resource"></a><span data-ttu-id="46913-102">Recurso ColumnDefinition</span><span class="sxs-lookup"><span data-stu-id="46913-102">ColumnDefinition resource</span></span>

## <a name="json-representation"></a><span data-ttu-id="46913-103">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="46913-103">JSON representation</span></span>

<span data-ttu-id="46913-104">Aqui está uma representação JSON de um recurso ColumnDefinition.</span><span class="sxs-lookup"><span data-stu-id="46913-104">Here is a JSON representation of a ColumnDefinition resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="46913-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="46913-105">Properties</span></span>

<span data-ttu-id="46913-106">O recurso **columnDefinition** tem as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="46913-106">The **columnDefinition** resource has the following properties.</span></span>

| <span data-ttu-id="46913-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="46913-107">Property name</span></span>           | <span data-ttu-id="46913-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="46913-108">Type</span></span>    | <span data-ttu-id="46913-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="46913-109">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="46913-110">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="46913-110">**columnGroup**</span></span>         | <span data-ttu-id="46913-111">string</span><span class="sxs-lookup"><span data-stu-id="46913-111">string</span></span>  | <span data-ttu-id="46913-112">Para colunas de site, o nome do grupo ao qual esta coluna pertence.</span><span class="sxs-lookup"><span data-stu-id="46913-112">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="46913-113">Ajuda a organizar as colunas relacionadas.</span><span class="sxs-lookup"><span data-stu-id="46913-113">Helps organize related columns.</span></span>
| <span data-ttu-id="46913-114">**description**</span><span class="sxs-lookup"><span data-stu-id="46913-114">**description**</span></span>         | <span data-ttu-id="46913-115">string</span><span class="sxs-lookup"><span data-stu-id="46913-115">string</span></span>  | <span data-ttu-id="46913-116">A descrição voltado para o usuário da coluna.</span><span class="sxs-lookup"><span data-stu-id="46913-116">The user-facing description of the column.</span></span>
| <span data-ttu-id="46913-117">**displayName**</span><span class="sxs-lookup"><span data-stu-id="46913-117">**displayName**</span></span>         | <span data-ttu-id="46913-118">string</span><span class="sxs-lookup"><span data-stu-id="46913-118">string</span></span>  | <span data-ttu-id="46913-119">O nome voltado para o usuário da coluna.</span><span class="sxs-lookup"><span data-stu-id="46913-119">The user-facing name of the column.</span></span>
| <span data-ttu-id="46913-120">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="46913-120">**enforceUniqueValues**</span></span> | <span data-ttu-id="46913-121">booliano</span><span class="sxs-lookup"><span data-stu-id="46913-121">boolean</span></span> | <span data-ttu-id="46913-122">Se for verdadeiro, esse mesmo valor não constará em dois itens de lista nessa coluna.</span><span class="sxs-lookup"><span data-stu-id="46913-122">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="46913-123">**hidden**</span><span class="sxs-lookup"><span data-stu-id="46913-123">**hidden**</span></span>              | <span data-ttu-id="46913-124">booliano</span><span class="sxs-lookup"><span data-stu-id="46913-124">boolean</span></span> | <span data-ttu-id="46913-125">Especifica se a coluna é exibida na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="46913-125">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="46913-126">**id**</span><span class="sxs-lookup"><span data-stu-id="46913-126">**id**</span></span>                  | <span data-ttu-id="46913-127">string</span><span class="sxs-lookup"><span data-stu-id="46913-127">string</span></span>  | <span data-ttu-id="46913-128">O identificador exclusivo da coluna.</span><span class="sxs-lookup"><span data-stu-id="46913-128">The unique identifier for the column.</span></span>
| <span data-ttu-id="46913-129">**indexed**</span><span class="sxs-lookup"><span data-stu-id="46913-129">**indexed**</span></span>             | <span data-ttu-id="46913-130">booliano</span><span class="sxs-lookup"><span data-stu-id="46913-130">boolean</span></span> | <span data-ttu-id="46913-131">Especifica se os valores da coluna podem ser usados para classificação e pesquisa.</span><span class="sxs-lookup"><span data-stu-id="46913-131">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="46913-132">**name**</span><span class="sxs-lookup"><span data-stu-id="46913-132">**name**</span></span>                | <span data-ttu-id="46913-133">string</span><span class="sxs-lookup"><span data-stu-id="46913-133">string</span></span>  | <span data-ttu-id="46913-134">O nome voltado para a API da coluna, conforme ele aparece nos [campos][] em uma [listItem][].</span><span class="sxs-lookup"><span data-stu-id="46913-134">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="46913-135">Para o nome voltado ao usuário, consulte **displayName**.</span><span class="sxs-lookup"><span data-stu-id="46913-135">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="46913-136">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="46913-136">**readOnly**</span></span>            | <span data-ttu-id="46913-137">bool</span><span class="sxs-lookup"><span data-stu-id="46913-137">bool</span></span>    | <span data-ttu-id="46913-138">Especifica se os valores da coluna podem ser modificados.</span><span class="sxs-lookup"><span data-stu-id="46913-138">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="46913-139">**required**</span><span class="sxs-lookup"><span data-stu-id="46913-139">**required**</span></span>            | <span data-ttu-id="46913-140">booliano</span><span class="sxs-lookup"><span data-stu-id="46913-140">boolean</span></span> | <span data-ttu-id="46913-141">Especifica se o valor da coluna não é opcional.</span><span class="sxs-lookup"><span data-stu-id="46913-141">Specifies whether the column value is not optional.</span></span>

<span data-ttu-id="46913-142">As colunas podem conter dados de vários tipos.</span><span class="sxs-lookup"><span data-stu-id="46913-142">Columns can hold data of various types.</span></span>
<span data-ttu-id="46913-143">As propriedades a seguir indicam qual tipo de dados uma coluna armazena, bem como configurações adicionais para esses dados.</span><span class="sxs-lookup"><span data-stu-id="46913-143">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="46913-144">Essas propriedades são mutuamente exclusivas: uma coluna só pode ter uma delas especificada.</span><span class="sxs-lookup"><span data-stu-id="46913-144">These properties are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="46913-145">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="46913-145">Property name</span></span>     | <span data-ttu-id="46913-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="46913-146">Type</span></span>                    | <span data-ttu-id="46913-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="46913-147">Description</span></span>
|:------------------|:------------------------|:-------------------------------
| <span data-ttu-id="46913-148">**boolean**</span><span class="sxs-lookup"><span data-stu-id="46913-148">**boolean**</span></span>       | <span data-ttu-id="46913-149">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="46913-149">[booleanColumn][]</span></span>       | <span data-ttu-id="46913-150">Esta coluna armazena valores boolianos.</span><span class="sxs-lookup"><span data-stu-id="46913-150">This column stores boolean values.</span></span>
| <span data-ttu-id="46913-151">**calculated**</span><span class="sxs-lookup"><span data-stu-id="46913-151">**calculated**</span></span>    | <span data-ttu-id="46913-152">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="46913-152">[calculatedColumn][]</span></span>    | <span data-ttu-id="46913-153">Os dados dessa coluna são calculados com base em outras colunas.</span><span class="sxs-lookup"><span data-stu-id="46913-153">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="46913-154">**choice**</span><span class="sxs-lookup"><span data-stu-id="46913-154">**choice**</span></span>        | <span data-ttu-id="46913-155">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="46913-155">[choiceColumn][]</span></span>        | <span data-ttu-id="46913-156">Esta coluna armazena dados de uma lista de opções.</span><span class="sxs-lookup"><span data-stu-id="46913-156">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="46913-157">**currency**</span><span class="sxs-lookup"><span data-stu-id="46913-157">**currency**</span></span>      | <span data-ttu-id="46913-158">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="46913-158">[currencyColumn][]</span></span>      | <span data-ttu-id="46913-159">Esta coluna armazena valores monetários.</span><span class="sxs-lookup"><span data-stu-id="46913-159">This column stores currency values.</span></span>
| <span data-ttu-id="46913-160">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="46913-160">**dateTime**</span></span>      | <span data-ttu-id="46913-161">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="46913-161">[dateTimeColumn][]</span></span>      | <span data-ttu-id="46913-162">Esta coluna armazena valores de datetime.</span><span class="sxs-lookup"><span data-stu-id="46913-162">This column stores DateTime values.</span></span>
| <span data-ttu-id="46913-163">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="46913-163">**defaultValue**</span></span>  | <span data-ttu-id="46913-164">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="46913-164">[defaultColumnValue][]</span></span>  | <span data-ttu-id="46913-165">O valor padrão dessa coluna.</span><span class="sxs-lookup"><span data-stu-id="46913-165">The default value for this column.</span></span>
| <span data-ttu-id="46913-166">**lookup**</span><span class="sxs-lookup"><span data-stu-id="46913-166">**lookup**</span></span>        | <span data-ttu-id="46913-167">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="46913-167">[lookupColumn][]</span></span>        | <span data-ttu-id="46913-168">Os dados dessa coluna são procurados por outra fonte no site.</span><span class="sxs-lookup"><span data-stu-id="46913-168">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="46913-169">**number**</span><span class="sxs-lookup"><span data-stu-id="46913-169">**number**</span></span>        | <span data-ttu-id="46913-170">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="46913-170">[numberColumn][]</span></span>        | <span data-ttu-id="46913-171">Esta coluna armazena valores numéricos.</span><span class="sxs-lookup"><span data-stu-id="46913-171">This column stores number values.</span></span>
| <span data-ttu-id="46913-172">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="46913-172">**personOrGroup**</span></span> | <span data-ttu-id="46913-173">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="46913-173">[personOrGroupColumn][]</span></span> | <span data-ttu-id="46913-174">Esta coluna armazena valores de Pessoa ou Grupo.</span><span class="sxs-lookup"><span data-stu-id="46913-174">This column stores Person or Group values.</span></span>
| <span data-ttu-id="46913-175">**text**</span><span class="sxs-lookup"><span data-stu-id="46913-175">**text**</span></span>          | <span data-ttu-id="46913-176">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="46913-176">[textColumn][]</span></span>          | <span data-ttu-id="46913-177">Esta coluna armazena valores de texto.</span><span class="sxs-lookup"><span data-stu-id="46913-177">This column stores text values.</span></span>

<span data-ttu-id="46913-178">Observação: essas propriedades correspondem à enumeração [SPFieldType][] do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="46913-178">Note: These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="46913-179">Enquanto os tipos mais comuns de campo são representados acima, essa API ainda faltam alguns.</span><span class="sxs-lookup"><span data-stu-id="46913-179">While the most common field types are represented above, this API is still missing some.</span></span>
<span data-ttu-id="46913-180">nestes casos, nenhuma das facetas do tipo de coluna serão preenchidas, e a coluna só terá as propriedades básicas.</span><span class="sxs-lookup"><span data-stu-id="46913-180">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="46913-181">Comentários</span><span class="sxs-lookup"><span data-stu-id="46913-181">Remarks</span></span>

<span data-ttu-id="46913-182">Os valores ColumnDefinitions e valores de campo para colunas `hidden` não são mostrados por padrão.</span><span class="sxs-lookup"><span data-stu-id="46913-182">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="46913-183">Para vê-los ao listar **columnDefinitions**, inclua `hidden` na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="46913-183">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="46913-184">Para vê-los ao exibir valores **field** em [listItems][listItem], inclua as colunas desejadas por nome na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="46913-184">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

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

<span data-ttu-id="46913-197">
  [SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx</span><span class="sxs-lookup"><span data-stu-id="46913-197">[SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition"
} -->
