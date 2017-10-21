---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ColumnDefinition
ms.openlocfilehash: e5942ddee4b505243cb64121862ce9e89e52d245
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="columndefinition-resource"></a><span data-ttu-id="dc37d-102">Recurso ColumnDefinition</span><span class="sxs-lookup"><span data-stu-id="dc37d-102">ColumnDefinition resource</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc37d-103">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dc37d-103">JSON representation</span></span>

<span data-ttu-id="dc37d-104">Aqui está uma representação JSON de um recurso ColumnDefinition.</span><span class="sxs-lookup"><span data-stu-id="dc37d-104">Here is a JSON representation of a {type} resource.</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnDefinition",
       "keyProperty": "id", "optionalProperties": [ ] } -->

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

## <a name="properties"></a><span data-ttu-id="dc37d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dc37d-105">Properties</span></span>

<span data-ttu-id="dc37d-106">O recurso **columnDefinition** tem as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="dc37d-106">The **columnDefinition** resource has the following properties.</span></span>

| <span data-ttu-id="dc37d-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="dc37d-107">Property name</span></span>           | <span data-ttu-id="dc37d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc37d-108">Type</span></span>    | <span data-ttu-id="dc37d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc37d-109">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="dc37d-110">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="dc37d-110">**columnGroup**</span></span>         | <span data-ttu-id="dc37d-111">string</span><span class="sxs-lookup"><span data-stu-id="dc37d-111">string</span></span>  | <span data-ttu-id="dc37d-112">Para colunas de site, o nome do grupo ao qual esta coluna pertence.</span><span class="sxs-lookup"><span data-stu-id="dc37d-112">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="dc37d-113">Ajuda a organizar as colunas relacionadas.</span><span class="sxs-lookup"><span data-stu-id="dc37d-113">Helps organize related columns.</span></span>
| <span data-ttu-id="dc37d-114">**description**</span><span class="sxs-lookup"><span data-stu-id="dc37d-114">**description**</span></span>         | <span data-ttu-id="dc37d-115">string</span><span class="sxs-lookup"><span data-stu-id="dc37d-115">string</span></span>  | <span data-ttu-id="dc37d-116">A descrição voltado para o usuário da coluna.</span><span class="sxs-lookup"><span data-stu-id="dc37d-116">The user-facing description of the column.</span></span>
| <span data-ttu-id="dc37d-117">**displayName**</span><span class="sxs-lookup"><span data-stu-id="dc37d-117">**displayName**</span></span>         | <span data-ttu-id="dc37d-118">string</span><span class="sxs-lookup"><span data-stu-id="dc37d-118">string</span></span>  | <span data-ttu-id="dc37d-119">O nome voltado para o usuário da coluna.</span><span class="sxs-lookup"><span data-stu-id="dc37d-119">The user-facing name of the column.</span></span>
| <span data-ttu-id="dc37d-120">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="dc37d-120">**enforceUniqueValues**</span></span> | <span data-ttu-id="dc37d-121">booliano</span><span class="sxs-lookup"><span data-stu-id="dc37d-121">boolean</span></span> | <span data-ttu-id="dc37d-122">Se for verdadeiro, esse mesmo valor não constará em dois itens de lista nessa coluna.</span><span class="sxs-lookup"><span data-stu-id="dc37d-122">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="dc37d-123">**hidden**</span><span class="sxs-lookup"><span data-stu-id="dc37d-123">**hidden**</span></span>              | <span data-ttu-id="dc37d-124">booliano</span><span class="sxs-lookup"><span data-stu-id="dc37d-124">boolean</span></span> | <span data-ttu-id="dc37d-125">Especifica se a coluna é exibida na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="dc37d-125">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="dc37d-126">**id**</span><span class="sxs-lookup"><span data-stu-id="dc37d-126">**id**</span></span>                  | <span data-ttu-id="dc37d-127">string</span><span class="sxs-lookup"><span data-stu-id="dc37d-127">string</span></span>  | <span data-ttu-id="dc37d-128">O identificador exclusivo da coluna.</span><span class="sxs-lookup"><span data-stu-id="dc37d-128">The unique identifier for the column.</span></span>
| <span data-ttu-id="dc37d-129">**indexed**</span><span class="sxs-lookup"><span data-stu-id="dc37d-129">**Indexed**</span></span>             | <span data-ttu-id="dc37d-130">booliano</span><span class="sxs-lookup"><span data-stu-id="dc37d-130">boolean</span></span> | <span data-ttu-id="dc37d-131">Especifica se os valores da coluna podem ser usados para classificação e pesquisa.</span><span class="sxs-lookup"><span data-stu-id="dc37d-131">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="dc37d-132">**name**</span><span class="sxs-lookup"><span data-stu-id="dc37d-132">**name**</span></span>                | <span data-ttu-id="dc37d-133">string</span><span class="sxs-lookup"><span data-stu-id="dc37d-133">string</span></span>  | <span data-ttu-id="dc37d-134">O nome voltado para a API da coluna, conforme ele aparece nos [campos][] em uma [listItem][].</span><span class="sxs-lookup"><span data-stu-id="dc37d-134">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="dc37d-135">Para o nome voltado ao usuário, consulte **displayName**.</span><span class="sxs-lookup"><span data-stu-id="dc37d-135">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="dc37d-136">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="dc37d-136">**Read-only.**</span></span>            | <span data-ttu-id="dc37d-137">bool</span><span class="sxs-lookup"><span data-stu-id="dc37d-137">bool</span></span>    | <span data-ttu-id="dc37d-138">Especifica se os valores da coluna podem ser modificados.</span><span class="sxs-lookup"><span data-stu-id="dc37d-138">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="dc37d-139">**required**</span><span class="sxs-lookup"><span data-stu-id="dc37d-139">**Required**</span></span>            | <span data-ttu-id="dc37d-140">booliano</span><span class="sxs-lookup"><span data-stu-id="dc37d-140">boolean</span></span> | <span data-ttu-id="dc37d-141">Especifica se o valor da coluna não é opcional.</span><span class="sxs-lookup"><span data-stu-id="dc37d-141">Specifies whether the column value is not optional.</span></span>

<span data-ttu-id="dc37d-142">As colunas podem conter dados de vários tipos.</span><span class="sxs-lookup"><span data-stu-id="dc37d-142">Columns can hold data of various types.</span></span>
<span data-ttu-id="dc37d-143">As propriedades a seguir indicam qual tipo de dados uma coluna armazena, bem como configurações adicionais para esses dados.</span><span class="sxs-lookup"><span data-stu-id="dc37d-143">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="dc37d-144">Essas propriedades são mutuamente exclusivas: uma coluna só pode ter uma delas especificada.</span><span class="sxs-lookup"><span data-stu-id="dc37d-144">These properties are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="dc37d-145">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="dc37d-145">Property name</span></span>     | <span data-ttu-id="dc37d-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc37d-146">Type</span></span>                    | <span data-ttu-id="dc37d-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc37d-147">Description</span></span>
|:------------------|:------------------------|:-------------------------------
| <span data-ttu-id="dc37d-148">**boolean**</span><span class="sxs-lookup"><span data-stu-id="dc37d-148">**Boolean**</span></span>       | <span data-ttu-id="dc37d-149">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="dc37d-149">[booleanColumn][]</span></span>       | <span data-ttu-id="dc37d-150">Esta coluna armazena valores boolianos.</span><span class="sxs-lookup"><span data-stu-id="dc37d-150">This column stores boolean values.</span></span>
| <span data-ttu-id="dc37d-151">**calculated**</span><span class="sxs-lookup"><span data-stu-id="dc37d-151">**Calculated**</span></span>    | <span data-ttu-id="dc37d-152">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="dc37d-152">[calculatedColumn][]</span></span>    | <span data-ttu-id="dc37d-153">Os dados dessa coluna são calculados com base em outras colunas.</span><span class="sxs-lookup"><span data-stu-id="dc37d-153">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="dc37d-154">**choice**</span><span class="sxs-lookup"><span data-stu-id="dc37d-154">**choice**</span></span>        | <span data-ttu-id="dc37d-155">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="dc37d-155">[choiceColumn][]</span></span>        | <span data-ttu-id="dc37d-156">Esta coluna armazena dados de uma lista de opções.</span><span class="sxs-lookup"><span data-stu-id="dc37d-156">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="dc37d-157">**currency**</span><span class="sxs-lookup"><span data-stu-id="dc37d-157">**Currency**</span></span>      | <span data-ttu-id="dc37d-158">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="dc37d-158">[currencyColumn][]</span></span>      | <span data-ttu-id="dc37d-159">Esta coluna armazena valores monetários.</span><span class="sxs-lookup"><span data-stu-id="dc37d-159">This column stores currency values.</span></span>
| <span data-ttu-id="dc37d-160">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="dc37d-160">**DateTime**</span></span>      | <span data-ttu-id="dc37d-161">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="dc37d-161">[dateTimeColumn][]</span></span>      | <span data-ttu-id="dc37d-162">Esta coluna armazena valores de datetime.</span><span class="sxs-lookup"><span data-stu-id="dc37d-162">This column stores DateTime values.</span></span>
| <span data-ttu-id="dc37d-163">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="dc37d-163">**DefaultValue**</span></span>  | <span data-ttu-id="dc37d-164">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="dc37d-164">[defaultColumnValue][]</span></span>  | <span data-ttu-id="dc37d-165">O valor padrão dessa coluna.</span><span class="sxs-lookup"><span data-stu-id="dc37d-165">The default value for this property is False.</span></span>
| <span data-ttu-id="dc37d-166">**lookup**</span><span class="sxs-lookup"><span data-stu-id="dc37d-166">**Lookup**</span></span>        | <span data-ttu-id="dc37d-167">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="dc37d-167">[lookupColumn][]</span></span>        | <span data-ttu-id="dc37d-168">Os dados dessa coluna são procurados por outra fonte no site.</span><span class="sxs-lookup"><span data-stu-id="dc37d-168">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="dc37d-169">**number**</span><span class="sxs-lookup"><span data-stu-id="dc37d-169">**number**</span></span>        | <span data-ttu-id="dc37d-170">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="dc37d-170">[numberColumn][]</span></span>        | <span data-ttu-id="dc37d-171">Esta coluna armazena valores numéricos.</span><span class="sxs-lookup"><span data-stu-id="dc37d-171">This column stores number values.</span></span>
| <span data-ttu-id="dc37d-172">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="dc37d-172">**personOrGroup**</span></span> | <span data-ttu-id="dc37d-173">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="dc37d-173">[personOrGroupColumn][]</span></span> | <span data-ttu-id="dc37d-174">Esta coluna armazena valores de Pessoa ou Grupo.</span><span class="sxs-lookup"><span data-stu-id="dc37d-174">This column stores Person or Group values.</span></span>
| <span data-ttu-id="dc37d-175">**text**</span><span class="sxs-lookup"><span data-stu-id="dc37d-175">**text**</span></span>          | <span data-ttu-id="dc37d-176">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="dc37d-176">[textColumn][]</span></span>          | <span data-ttu-id="dc37d-177">Esta coluna armazena valores de texto.</span><span class="sxs-lookup"><span data-stu-id="dc37d-177">This column stores text values.</span></span>

<span data-ttu-id="dc37d-178">Observação: essas propriedades correspondem à enumeração [SPFieldType][] do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="dc37d-178">Note: These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="dc37d-179">Embora os tipos de campo mais comuns estejam representados acima, ainda falta alguns a essa API beta.</span><span class="sxs-lookup"><span data-stu-id="dc37d-179">While the most common field types are represented above, this beta API is still missing some.</span></span>
<span data-ttu-id="dc37d-180">nestes casos, nenhuma das facetas do tipo de coluna serão preenchidas, e a coluna só terá as propriedades básicas.</span><span class="sxs-lookup"><span data-stu-id="dc37d-180">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="dc37d-181">Comentários</span><span class="sxs-lookup"><span data-stu-id="dc37d-181">Remarks</span></span>

<span data-ttu-id="dc37d-182">Os valores ColumnDefinitions e valores de campo para colunas `hidden` não são mostrados por padrão.</span><span class="sxs-lookup"><span data-stu-id="dc37d-182">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="dc37d-183">Para vê-los ao listar **columnDefinitions**, inclua `hidden` na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="dc37d-183">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="dc37d-184">Para vê-los ao exibir valores **field** em [listItems][listItem], inclua as colunas desejadas por nome na instrução `$select`.</span><span class="sxs-lookup"><span data-stu-id="dc37d-184">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

[booleanColumn]: booleanColumn.md
[calculatedColumn]: calculatedColumn.md
[choiceColumn]: choiceColumn.md
[currencyColumn]: currencyColumn.md
[dateTimeColumn]: dateTimeColumn.md
[defaultColumnValue]: defaultColumnValue.md
[lookupColumn]: lookupColumn.md
[numberColumn]: numberColumn.md
[personOrGroupColumn]: personOrGroupColumn.md
[textColumn]: textColumn.md
[fieldValueSet]: fieldValueSet.md
[fields]: fieldvalueset.md
[listItem]: listitem.md

[SPFieldType]: https://msdn.microsoft.com/en-us/library/microsoft.sharepoint.spfieldtype.aspx

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition"
} -->
